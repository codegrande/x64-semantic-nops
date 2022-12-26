# Semantic NOPs for x64 architecture
Copyright 2021-2022 Philippe Paquet

---

### Description

Semantic NOPs are machine language instructions or combinations of machine language instructions that have no effect other than advancing the instruction pointer. They are used for obfuscation. This collection is presented as a set of json files:
- x64_semantic_nops_1_byte.json
- x64_semantic_nops_2_bytes.json
- x64_semantic_nops_3_bytes.json
- x64_semantic_nops_4_bytes.json
- x64_semantic_nops_5_bytes.json
- x64_semantic_nops_6_bytes.json
- x64_semantic_nops_8_bytes.json
- x64_semantic_nops_all.json

Files are formated as following:
```json
{
    "nops_count": 1,
    "nops": [
        {
            "asm_count": 1,
            "asm": [
                "nop"
            ],
            "hex_count": 1,
            "hex": "90"
        }
    ]
}
```

`nops_count`: number of NOPs in the file  
`nops`: array containing the NOPs  
`asm_count`: number of instructions for the NOP  
`asm`: array of instructions for the NOP  
`hex_count`: number of bytes for the NOP  
`hex`: bytes for the NOP as a string of hexadecimal values separated by a space  

---

### Contributing

Bug reports and suggestions for improvements are most welcome.

---

### Contact

If you have any questions, comments or suggestions, do not hesitate to contact me at philippe@paquet.email
