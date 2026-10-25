# Streaminzito 

*Streaminzito* is a video specialized RTS (Receive Transform Send), is like a streaming ETL (Extract Transform Load) service.

It receive video streaming, transform the source executing a certain module (plug-and-play) on it and stream back.

*Streaminzito* has 2 channels:
- Receive channel
- Send channel

## Key Architectural Choice
- comunication is asynchronous, 1:N = streaminzito:client.
- no inbound queue

## Technology Stack
- Async Runtime: [tokio](https://github.com/tokio-rs/tokio) 
- RTC: [st0rm](https://github.com/algesten/str0m)