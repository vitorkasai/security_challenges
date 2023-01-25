# Modo de Operação CTR
- O modo de operação counter transforma uma cifra de bloco em uma cifra de fluxo.
- Usa um contador.
- Em cada iteração o contador é incrementado.
- O nonce é combinado com o contador usando alguma operação reversível para produzir um único bloco para encrypt.
- O tamanho do bloco do contador é o mesmo que o do plaintext.
- Não é seguro repetir o mesmo nonce com a mesma chave.

![wikipedia ctr um](https://github.com/42kkkkkaren/security_challenges/blob/main/Challenge%2018/pictures/reschallenge181)

- Se você descobre o plain text correspondente ao cipher text de uma mensagem com uma keystream, é possível decriptar qualquer outra mensagem criptografada com o mesmo keystream.
- O decrypt é realizado da mesma forma que o encrypt:

![wikipedia ctr dois](https://github.com/42kkkkkaren/security_challenges/blob/main/Challenge%2018/pictures/reschallenge182)

- O XOR é realizado com o cipher text, gerando o plaintext.
