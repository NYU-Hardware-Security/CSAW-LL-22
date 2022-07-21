
# CSAW Logic Locking Conquest 2022
[Competition website](https://sites.google.com/nyu.edu/csaw-llc-2022/home) - [Register now](https://sites.google.com/nyu.edu/csaw-llc-2022/register)
## Aims of the challenge
** Backgroud** 
Logic Locking is a revolutionary technique for protecting Intellectual Property of Integrated Circuits from myriad security threats, such as reverse engineering, overbuilding, piracy, and hardware Trojan insertion. In this student-led Logic Locking Conquest Challenge, participants will attempt to attack designs locked with [ASSURE](https://www.google.com/url?q=https://arxiv.org/abs/2010.05344&sa=D&sntz=1&usg=AOvVaw0pfCWeveAukQ6CbJCcCzmd), a state-of-the-art RTL locking technique. This year's challenge emphasizes the assessment of large designs (large IPs, large "keys").

In previous years, CSAW LL has featured FPGA-based Redaction, Sequential Locking/Obfuscation, and SAT-resilient locking.

This year's challenge focuses on the locking techniques provided by [ASSURE](https://www.google.com/url?q=https%3A%2F%2Farxiv.org%2Fabs%2F2010.05344&sa=D&sntz=1&usg=AOvVaw0pfCWeveAukQ6CbJCcCzmd). The designs you will be given have been locked at register transfer level and then synthesized.

The red teams will compete to recover locked designs and will be judged on how many designs they attack, the success of those attacks (based on the criteria below), and the quality of their technical write-up and presentation.

**Evaluation Criteria:---**

Your submission will be evaluated based on your approach to find the following assets of the locked designs:

-   **Finding the unlocking key**: Find the key that unlocks the design: scored will be given depending on the threat model (Oracle-guided less points /Oracle-less more points) and scan chain access (0%-50%-100%, the more access the less points) .
    
-   **Reverse engineering of the design**: Identify what the locked design implements. For this task you are required to submit a report describing your approach (manual inspection/ existing tools/ developed tools) and your findings. The more accurate are the findings the higher the score. This task is evaluated only in an oracle-less scenario.
As a warm up, you have access to a toy “example” that directs you towards the self-evaluation of your attack. A (text) tutorial is also provided to walk you through the example and introduce you to the steps to follow while evaluating.

**Evaluation Criteria:---**

Your submission will be evaluated based on your approach to find the following assets of the locked designs:

-   **Finding the unlocking key**: Find the key that unlocks the design: scored will be given depending on the threat model (Oracle-guided less points /Oracle-less more points) and scan chain access (0%-50%-100%, the more access the less points) .
    
-   **Reverse engineering of the design**: Identify what the locked design implements. For this task you are required to submit a report describing your approach (manual inspection/ existing tools/ developed tools) and your findings. The more accurate are the findings the higher the score. This task is evaluated only in an oracle-less scenario.
    

**Deliverables:---**

**Technical Report:** To submit your findings you must provide a comprehensive report. The report must include the following technical details:
    

-   Detailed assumptions on the considered thread model.
    
-   Your findings on the locked designs for each considered threat model
    
     -   If your attack focused on retrieving the unlocking key, in the findings it is sufficient to report the retrieved key;
                    
     -   If your attack focused on reverse engineering the locked design, in your findings you should have a description of what was the original functionality of the locked design (the more details the better).
       

Example (Assume the original design was an AES core):  
Unlocking key: XXXXX  
Reverse engineering: the original design implemented a block cipher with 128 bit key and 128 bit block size.  
Reverse engineering (better report): the original design implemented an aes core with 128 bit key

-   Detailed algorithm/strategy behind your attacking approach. If possible, provide your setup (along with binary, instructions, etc.) to reproduce the results by the blue-team.
-   Any other assumptions being made.
-   Any shortcomings of your approach (in case you are unable to extract what you desired to).

## Additional details
This repo will be used to publish the benchmarks for the two phases of the competition. If you signed up for the competition you will be notified when we upload new material.
