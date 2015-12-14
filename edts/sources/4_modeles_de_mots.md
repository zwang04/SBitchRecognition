A phonetic dictionary contains a mapping from words to phones. This mapping is not very effective. For example, only two to three pronunciation variants are noted in it, but it's practical enough most of the time. The dictionary is not the only variant of mapper from words to phones. It could be done with some complex function learned with a machine learning algorithm. 

Le modèle de mot est la dictonaire phonétique qui contiens a map des mot et des chaines de caractère correspondants.

Franchement dit, notre dictionaire n'est pas hyper efficace. Par exemple, il y a qu'une pronunciation variante (2 ou 3 pour certaines mots) est noté dans le dictionaire pour chaque mot, mais c'est pratique à utiliser plupart de temps, surtout quand on a pas trop de temps a réaliser notre programme.

Heuresement, la dictionaire n'est pas la seul map qui contiens des mots comme key et des prononciation comme value. Il pourra également être fait par des function complex qui prenne un alogrithme de machine learning.


There are various tools to help you to extend an existing dictionary for new words or to build a new dictionary from scratch. If your language already has a dictionary it's recommended to use since it's carefully tuned for best performance. If you starting a new language you need to account for various reductions and coarticulations effects. They make it very hard to create accurate rules to convert text to sounds. However, the practice shows that even naive conversion could produce a good results for speech recognition. For example, many developers were successful to create ASR with simple grapheme-based synthesis where each letter is just mapped to itself not to the corresponding phone.

For most of the languages you need to use specialized grapheme to phoneme (g2p) code to do the conversion using machine learning methods and existing small database. Nowdays most accurate g2p tools are Phonetisaurus: 
