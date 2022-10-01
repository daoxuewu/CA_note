# 計算機組織整理

# Chapter 1 

## basic concept

計算機的 **命令(commands)** 在高階語言中稱為**敘述(statments)**(eg. p = x + y\*z)，在低階語言中稱為**指令(instructions)**\(eg. add $s0, $s1, $s2)。

指令是CPU可以執行的最基本運算(primitive operation)，而一步計算機所可以執行的指令的集合就稱為**指令集(instruction set)**。

使用相同指令集所建構的CPIs彼此是**相容的(compatible)**

學習低階語言所須了解的基本硬體架構(Hardware Information)及指令集稱為**指令集架構**(Instruction Set Architecture,ISA)

## MIPS introduction

CPU一次可以處理的資料量稱為一個**字組(word)**,一個字組是16bits、32bits、64bits等。如果某個CPU可以處理的字組大小為32bits，則我們稱此CPU為32bits的CPU。依據MIPS R2000指令集所造出來的CPU也是一個32bits的CPU。

CPU一次可以處理的資料量也可以由一些硬體的規格看出端倪，例如一個32bits的CPU其一般目的**暫存器(general purpose register)**、**ALU**也都是32bits。

### RISC vs CISC
ISA以1980年為分界，1980為RISC(速度較快)

RISC : 精簡指令集，代表指令數很少，而且只提供簡單的基本指令，目的是希望造出來的計算機能夠比較簡單一些，執行指令速度能夠快一些

CISC : 複雜指令集，指令數多，除了提供簡單的基本指令之外還提供功能強大的複雜指令，目的在提供較佳的程式設計環境以減輕programmer的負擔。

(背)Intel 80x86,AMD Opteron based on CISC.

## ISA 

### Hardware Information
1. Memory
2. Register
4. Instruction format
5. Addressing mode

### Basic Computer Structure
1. Control unit
2. Datapath
3. Memory
4. Input device
5. Output device



## 題目中出現的英文單字
abstraction (n) : 抽象
enable (v) : to make someone able to do something, or to make something possible
identical (a) : exactly the same, or very similar
term (n) : 術語，專門名稱
memory : 
- 功能是儲存正在執行中的程式，包含他的data跟instructions(一連串的instructions就叫做code)
- 把Memory當成一個大櫃子，每一個抽屜都有編號(address)，抽屜裡可以放東西(content)

**CPU : control unit + datapath**
**datapath** : CPU裡面的一個電路，是真正執行instruction，處理data的地方 = **ALU + Registers** (交大資聯考過，課本前後定義不一，考試時以這個定義為準)
ALU : 負責執行算數邏輯運算
Registers : 存要運算的運算元和運算的結果



