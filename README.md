import pathlib
from pathlinb import Path
import json

while True:
    nome=input('digite seu nome ou sair para encerrar\n >>> ')
    if nome.lower()=="sair":
        print('fim do programa.')
        break
    if not nome:
        print('entrada invalida nome não pode ser vazio!!!')
        continue

   path=Path('nome.json')
   conteudo=json.dumps("nome")
   path.write_text('conteudo')

   print(f
