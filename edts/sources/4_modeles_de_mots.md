Le modèle de mot est la dictonaire phonétique qui contiens une map des mot et des chaines de caractère correspondants.

Franchement dit, notre dictionaire n'est pas hyper efficace. Par exemple, il y a qu'une pronunciation variante (2 ou 3 pour certaines mots) est noté dans le dictionaire pour chaque mot, mais c'est pratique à utiliser aux plupart de temps, surtout quand on a pas trop de temps a réaliser notre programme.

Heuresement, la dictionaire n'est pas la seul map qu'on pourra avoir qui contiens des mots comme key et des prononciation comme value. Il pourra également être fait par des function complex qui prenne un alogrithme de machine learning.

Création de dictionaire:

Il existe plusieur outils qui permettent de générer une dictionnaire de rien ou d'extendre une dictionnaire existante.

Si vous voulez générer une dictionnaire, vous devait penser à des réductions et des effets de coarticulation. Ils sont complex pour créer des régles exactes pour convertir les text au prononciation.

Pour plupart de language, on doit utiliser des code grapheme to phoneme (g2p) spécialisé pour faire la conversion en utilisant des méthodes machine learning et des petit database existant:

 est le g2p assez correct.   
blabalabala

On a toujours besoin de TTS(text to sppech) (speech synthesis system). Il est souvent plus extensif que requise pour Automatique speech recongnition, et en même temps il a un grande avantage qu'il fourni beaucoup plus de fonctionnalité que les G2P simple.

Par exemple, ils peuvent faire tokenization, qui est une processus de tranformer des streams à des mots, des phrases, des symbol, ou des autres élément, par convertir des chiffres et des abbreviations à format parole.

A phonetic dictionary contains a mapping from words to phones. This mapping is not very effective. For example, only two to three pronunciation variants are noted in it, but it's practical enough most of the time. The dictionary is not the only variant of mapper from words to phones. It could be done with some complex function learned with a machine learning algorithm.

There are various tools to help you to extend an existing dictionary for new words or to build a new dictionary from scratch. If your language already has a dictionary it's recommended to use since it's carefully tuned for best performance. If you starting a new language you need to account for various reductions and coarticulations effects. They make it very hard to create accurate rules to convert text to sounds. However, the practice shows that even naive conversion could produce a good results for speech recognition. For example, many developers were successful to create ASR with simple grapheme-based synthesis where each letter is just mapped to itself not to the corresponding phone.

For most of the languages you need to use specialized grapheme to phoneme (g2p) code to do the conversion using machine learning methods and existing small database.

Please note that if you use TTS you often need to do phoneset conversion. TTS phonesets are usually more extensive than required for ASR. However, there is a great adavantage in TTS tools because they usually contain more required functionality than simple G2P. For example, they are doing tokenization by converting numbers and abbreviations to spoken format. 
