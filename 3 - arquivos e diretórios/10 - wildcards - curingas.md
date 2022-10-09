# Wildcards (curingas)

- * (asteristico)
    - significa tudo que for isso que eu to dizendo
    - o * também complementa dizendo que tudo que começar com essa letra é pra pegar e executar a ação

$ mv fi* pasta1
- movi tudo que começãva com fi e copiei pra pasta um


$ mv fi* ../
- movi tudo que começava com fi para um diretório anterior a esse onde os arquivos se encontravam



- ? (interrogação)
    - completa até 1 caractere

$ mv pasta? vem

nesse caso, eu tinha uma lista de pastas: pasta 1 pasta2 pasta3...
e eu disse pra ele pegar tudo que tiver pasta(? e mas um número, por exemplo), era pra mover pra pasta vem.. 
- essa interrogação serve pra quando vc tem vários arquivos de mesmo nome e que só muda o final deles.. aí da pra pegar e mover pra ouro lugar

$ rm -r pasta?
removi tudo que era pasta? (pasta + alguma coisa)

OBS:

- 1: se tiver mais de um caractere depois da palavra que vc disse, ele vai desconsiderar. 
- 2: se tiver um arquivo que já é o nome que vc colocou antes da insterrogação (pasta?) ele também vai desconsiderar. tem que ser pasta + 1 caractere

