# HASH-MD5
🧪 LAB - GERAR E ANALISAR O HASH MD5 
🎯 Objetivo
O objetivo deste projeto é demonstrar como gerar e verificar o hash MD5 de arquivos utilizando a ferramenta CertUtil, disponível no Microsoft Windows. A comparação dos hashes permite verificar se um arquivo permaneceu íntegro ou se sofreu alguma alteração.

🛠️ Ferramentas
Sistema Operacional: Microsoft Windows 10
Prompt de Comando (CMD)
CertUtil (utilitário nativo do Windows)

⚙️ Comando utilizado
Foram executados os seguintes comandos no Prompt de Comando:

certutil -hashfile "D:\Usuários\Diego\Downloads\imagem sensor.jpeg" MD5
certutil -hashfile "D:\Usuários\Diego\Downloads\imagem sensor1.jpeg" MD5
certutil -hashfile "D:\Usuários\Diego\Downloads\imagem sensor.jpeg" MD5
Resultados

Os hashes MD5 obtidos foram:

imagem sensor.jpeg → d682a609a4f304765e4926c9ab3f040d
imagem sensor1.jpeg → a22e2857c40fb7543ea784d3e764965e
imagem sensor.jpeg (nova verificação sobreescrevendo o arquivo) → 442ede3493d452f12738db47a15eadc0

## 📊 Resultado obtido

Durante a execução do comando certutil -hashfile, foram gerados os hashes MD5 dos arquivos analisados. O arquivo imagem sensor.jpeg apresentou inicialmente o hash d682a609a4f304765e4926c9ab3f040d, enquanto o arquivo imagem sensor1.jpeg apresentou o hash a22e2857c40fb7543ea784d3e764965e.

Na terceira execução, ao calcular novamente o hash do arquivo imagem sensor.jpeg, após sobreescrever o arquivo com a cópia, foi obtido o valor 442ede3493d452f12738db47a15eadc0, diferente do primeiro. Esse resultado demonstra que o conteúdo do arquivo foi alterado entre as duas verificações, pois qualquer modificação em um arquivo gera um hash MD5 diferente.

Assim, foi possível comprovar a utilidade do algoritmo MD5 para verificar a integridade de arquivos e identificar alterações em seu conteúdo.
