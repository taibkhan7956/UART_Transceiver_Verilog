# UART_Transceiver_Verilog
UART Transmitter and Receiver in Verilog with Baud Generator and Testbench
# UART Transceiver (Verilog/SystemVerilog)

This project implements a **UART (Universal Asynchronous Receiver Transmitter)** Transceiver using Verilog/SystemVerilog.  
It includes a **UART Transmitter**, **UART Receiver**, **Baud Rate Generator**, and a **Testbench** for simulation.

---

## 📌 Features

✅ UART Transmitter (TX)  
✅ UART Receiver (RX)  
✅ Baud Rate Generator for TX and RX  
✅ 8-bit data transmission  
✅ Start bit + 8 data bits + Stop bit  
✅ Receiver uses **16x oversampling** for better accuracy  
✅ Testbench with loopback (TX connected to RX)  
✅ Waveform support (VCD dump)

---

## 📂 Project Files

| File Name | Description |
|----------|-------------|
| `uart_baud_rate_gen.sv` | Generates baud enable pulses for TX and RX |
| `transmitter.sv` | UART transmitter module |
| `uart_receiver.sv` | UART receiver module with oversampling |
| `uart_top.sv` | Top module integrating TX + RX + baud generator |
| `testbench.sv` | Testbench for UART top module (loopback testing) |

---

## ⚙️ UART Configuration

- **Data Bits:** 8  
- **Start Bit:** 1 (logic 0)  
- **Stop Bit:** 1 (logic 1)  
- **Parity:** None  
- **Baud Rate (TX):** 9600 (assuming 50 MHz clock)  
- **Receiver Sampling:** 16x oversampling  

---



