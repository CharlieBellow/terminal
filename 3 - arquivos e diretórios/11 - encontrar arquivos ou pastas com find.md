# find

- encontrar arquivos ou diretórios

find <path> arg [expression]

* -type <d | f> 
* -name

como se lê:
encontre <nesse diretório> d (um diretŕio) | f (ou um arquivo) -name (com esse nome) "nome do arquivo que eu quero"


exemplo:
find . -type f -name "*.txt"
- pedi pra encontrar no meu diretorio atual um arquivo que tenha qualquer nome(*) desde que seja .txt

$ find home/charlie/Documentos -type d -name "*e*"
- pedi pra encontrar nesse diretório específico um diretório/pasta que tenha qualquer coisa antes(*)+ a letra e + qualqier coisa depois(*)

$ find . -type d -iname "*v*"
- com o iname dá pra procurar com eltras maiúsculas e minúsculas


// só funciona para buscar nome de arquivo ou extensão. não acha pelo conteúdo do arquivo.

Buscar a palavra "cesar" em nomes de arquivos, diretório e dentro de arquivos, a partir do diretório "/home":
dir="/home"; kw="cesar"; find $dir -name $kw*; grep -iR $kw $dir | grep -v "\/\./*";

Buscar a palavra "cesar" em nomes de arquivos, diretório e dentro de arquivos, a partir do diretório atual
dir=""; kw="cesar"; find $dir -name $kw*; grep -iR $kw $dir | grep -v "\/\./*";

se quiser achar os conteúdos dentro dos arquivos pode usar o programa catfish ou recall