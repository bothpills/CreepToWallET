# CreepToWallET
Carteira de criptomoedas 


Este código é uma implementação simples de uma carteira criptográfica usando JavaScript e a biblioteca BitcoinJS, com base no curso "Especialista em Blockchain" da Digital Innovation ONE. O código gera uma carteira determinística hierárquica (HD) para a rede Bitcoin Testnet, o que significa que ele cria uma carteira que pode gerar vários pares de chave pública e privada a partir de uma única frase-semente.


Dependências:

As seguintes dependências são necessárias para executar este código:
bip32: Esta é uma biblioteca que implementa o padrão BIP32 para criação de carteiras HD.
bip39: Esta é uma biblioteca que implementa o padrão BIP39 para geração de frases-semente mnemônicas.
bitcoinjs-lib: Esta é uma biblioteca que implementa criptografia e funcionalidades de transação relacionadas ao Bitcoin.


Rede:

Este código é configurado para gerar uma carteira para a rede Bitcoin Testnet, que é uma rede separada da rede principal do Bitcoin usada para fins de teste.


Carteira HD:

O código cria uma carteira HD derivando uma chave raiz a partir de uma frase-semente mnemônica gerada aleatoriamente usando o padrão BIP32. A partir desta chave raiz, um caminho de derivação específico é definido para criar uma conta específica. Neste caso, o caminho m/49'/1'/0'/0 é usado para gerar um endereço SegWit P2SH-P2WPKH. O código então deriva um nó específico desta conta para gerar um par de chave pública e privada.


Saída:

O código gera as seguintes informações:
O endereço da carteira gerada na rede Testnet Bitcoin
A chave privada associada ao endereço gerado
A frase-semente usada para gerar a carteira


Uso:

Para usar este código, você pode copiá-lo e colá-lo em um arquivo JavaScript e executá-lo usando o Node.js. Certifique-se de instalar as dependências necessárias antes de executar o código. Depois de executar o código, o endereço da carteira, a chave privada e a frase-semente gerada serão impressos no console.

