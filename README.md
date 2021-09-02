# A Benchmark Suite of RT-level Hardware Trojans for Pipelined Microprocessor Cores



Trojan Benchmarks Description

| Name       | Location           | Trigger                                                              | Payload                                     | Category  |  
|------------|--------------------|----------------------------------------------------------------------|---------------------------------------------|-----------|
| OR1K-T100  | Decode Unit        | Sequence of instructions                                             | Periodically forcing signal values          | DP        |
| OR1K-T200  | Control Unit       | Counters monitoring read accesses to SPRs                            | Entering the supervisor mode                | DoS       |
| OR1K-T300  | PIC Unit           | Counters for mask and status reg. write access                       | Disabling external interrupts               | CF        |
| OR1K-T400  | Control Unit       | 3 counters for monitoring instructions                               | Disabling control flag bit                  | CF        |
| OR1K-T500  | Decode Unit        | A specific sequence of instructions                                  | Introducing "bubbles" to stall the pipeline | DP        |
| OR1K-T600  | Data Cache         | Counters monitoring Data Cache Final State Machine (FSM) transitions | Invalidating dcache content                 | DP        |
| OR1K-T700  | Load & Store Unit  | Instruction type, order and number                                   | Exception on the data bus                   | DoS       |
| OR1K-T800  | Instr. Cache       | Counters monitoring Instr. Cache FSM transitions                     | Invalidating icache content                 | DoS       |





Copyright © 2021 Aleksa Damljanovic * Annachiara Ruospo

RTL Suite of Hardware Trojan Benchmarks for Pipelined Microprocessor Cores is a free and open-source set of benchmark designs and it is distributed under the permissive Apache-2.0 license.
