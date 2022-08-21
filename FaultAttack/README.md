# README #
Fault Analysis on the 9th round of AES

### INPUTS###
- data.txt : includes the correct ciphertext and the faulty ciphertext (9th round attack)
For example,
3cc9b867f400567bdaeffa49d524829e,e9f2e4203cf8ba1eb08c4856c6774f1e # Test for AES. Its input and corresponding ciphertext
5d639a745a3b031c931c0f32306ebc36,f2639a745a3b0390931c88323095bc36 # correct and faulty ciphertext, with fault in column 1 at start of Round 9
262e32bf47a940cb4db14053995900a6,26ef32bf61a940cb4db1406d995902a6 # correct and faulty ciphertext, with fault in column 2 at start of Round 9
de07169146197e15f6b892c0bda1f2fb,de07fc91468b7e1541b892c0bda1f20e # correct and faulty ciphertext, with fault in column 3 at start of Round 9
3bc129f8a6d18f1f074250838575b90f,3bc12937a6d1b51f07df50839b75b90f # correct and faulty ciphertext, with fault in column 4 at start of Round 9


The first line is the plaintext and corresponding correct ciphertext
The 2nd, 3rd, 4th, and 5th lines correspond to a correct ciphertext and a faulty ciphertext.
Each faulty ciphertext corresponds to a fault in each column. For instance, 2nd row corresponds
to a fault injected in the beginning of the 9th round in Column 1. 

- data4.txt : includes 8 pairs of correct and faulty ciphertexts
For example,
75a9c13e29bda0904181de983a2117bf,f58f293450bc8120d99860623f1b6aae #Test for AES. Its input and corresponding ciphertext
a9077d4a3add4c56c206d616c4a3000b,84077d4a3add4c93c2064616c48e000b # correct and faulty ciphertext, with fault in column 1 at start of Round 9
9b6a8606347c972d3bb8ff3a836d5471,9b388606d27c972d3bb8ff87836d5171 # correct and faulty ciphertext, with fault in column 2 at start of Round 9
2d9ee92f83f7b1d9235ea49a6dd1aaf5,2d9e082f8391b1d9a35ea49a6dd1aaa1 # correct and faulty ciphertext, with fault in column 3 at start of Round 9
a2a6309ee4bd08fd84f4cf7cc87fdcbe,a2a63037e4bddbfd84dfcf7cb47fdcbe # correct and faulty ciphertext, with fault in column 4 at start of Round 9
bcb767917c2f4cc3294d2ba313e76018,f7b767917c2f4cd4294d3aa313f46018 # correct and faulty ciphertext, with fault in column 1 at start of Round 9
d608fa5468e9b794814056fbce69a4dd,d68bfa5408e9b794814056d2ce6978dd # correct and faulty ciphertext, with fault in column 2 at start of Round 9
a7f67daaa3c5c8506d31029a8319ea14,a7f688aaa38dc8504b31029a8319ea6a # correct and faulty ciphertext, with fault in column 3 at start of Round 9
5d639a745a3b031c931c0f32306ebc36,f2639a745a3b0390931c88323095bc36 # correct and faulty ciphertext, with fault in column 4 at start of Round 9




- dfa_9vi.py : Offline phase for 9th round attack
 
### Execution Step###
 
python3 dfa_9vi.py -round 9 -input data.txt
 

