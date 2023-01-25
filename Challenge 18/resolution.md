# Modo de Operação CTR
- O modo de operação counter transforma uma cifra de bloco em uma cifra de fluxo.
- Usa um contador.
- Em cada iteração o contador é incrementado.
- O nonce é combinado com o contador usando alguma operação reversível para produzir um único bloco para encrypt.
- O tamanho do bloco do contador é o mesmo que o do plaintext.
- Não é seguro repetir o mesmo nonce com a mesma chave.

/assets/images/reschallenge181.png

- Se você descobre o plain text correspondente ao cipher text de uma mensagem com uma keystream, é possível decriptar qualquer outra mensagem criptografada com o mesmo keystream.
- O decrypt é realizado da mesma forma que o encrypt:

/assets/images/reschallenge182.png

- O XOR é realizado com o cipher text, gerando o plaintext.
