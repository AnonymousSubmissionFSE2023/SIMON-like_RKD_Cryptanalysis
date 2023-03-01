# SIMON-like_RKD_Cryptanalysis
**`Title`**：Related-key Differential Cryptanalysis of SIMON and SIMECK  
**`Author`**: Anonymous Submission   
**`Abstract`**： Although the differential behavior of SIMON and SIMECK has been extensively studied in the single-key scenario, their security against related-key attacks remains insufficiently understood. In this paper, we investigate the related-key differential (RKD) characteristics of SIMON and SIMECK. We first find that some RKD characteristics for these ciphers under the Markov cipher assumption may not always be valid. To address this issue, we develop an SMT model capable of finding good RKD characteristics and extracting the right pairs to ensure validity. Our model successfully reproduces and corrects all the best 15, 19, and 23 rounds of RKD characteristics reported for SIMECK and generates full-round RKD characteristics for SIMECK48/96 and SIMECK64/128, as well as extended RKD characteristics for SIMECK32/64. Additionally, we present optimal rotational-XOR differential characteristics for SIMECK32/64, 48/96, and 64/128, covering 24, 35, and 44 (full) rounds, respectively, which represent a significant improvement over the previous best results of 21, 28, and 35 rounds. These characteristics indicate that the security of SIMECK against related-key attacks is not as strong as claimed by the designers, and that there is a significant gap between the real case and what was previously believed. The full-round characteristics show that while there are similarities between SIMON and SPECK, the security reduction from SIMECK to that of SIMON and SPECK may not be straightforward.   
We then analyze the related-key characteristics of SIMON. The analysis requires significantly more computational resources and is more challenging than the corresponding analysis for SIMECK. Thus, we incorporate manually explored information into our model. For SIMONn2n/4n, we use iterative key differences to construct up to 19-round optimal iterative differences, which are the most effective distinguishers against SIMON32/64 and SIMON48/96. For cases where iterative differences are ineffective, we employ a combination of short-round distinguishers to obtain longer ones. Consequently, our paper presents the current longest valid distinguishers for all ten variants of SIMON in the related-key scenario. It is worth noting that the proposed RKD distinguishers for the larger version of SIMON96/96, 96/144, 128/128, 128/192, and 128/256 are for the first time in the decade since SIMON's publication.   
Finally, since SIMECK achieved a more compact and efficient design compared to SIMON by decreasing the rotation parameters from (8,1,2) to (5,0,1) and replacing the SIMON's key schedule with a Speck-style key schedule, we investigate the influence of the rotation parameters on related-key differential attacks for SIMECK. Our experiments show that replacing the rotation parameters does not significantly improve its resistance against related-key differential attacks. On the other hand, we introduce a new key schedule algorithm by adding a simple component to the existing key schedule. The modified SIMECK key schedule significantly enhances the resistance to related-key differential attacks compared to the standard simon and SIMECK, while maintaining most of the implementation advantage over SIMON.
