📦 Módulos e Pacotes no Python
Este guia explica, de forma simples, como organizar código em módulos e pacotes no Python, facilitando a manutenção e evitando que tudo fique em um único arquivo.

🔹 Módulos
Um módulo é um arquivo .py que contém funções, classes ou variáveis para serem reutilizadas em outros arquivos.

Por que usar módulos?
Evita arquivos muito grandes e confusos.

Facilita a manutenção do código.

Permite reutilizar funções em diferentes partes do programa.

📌 Exemplo de Estrutura
main.py     # Arquivo principal
func.py     # Arquivo com funções
📥 Importando um módulo — import

import func

func.somar(2, 3)
O import carrega todas as funções do módulo, o que pode consumir mais memória em projetos grandes.

📥 Importando funções específicas — from
from func import somar

somar(2, 3)
O from importa apenas as funções desejadas, tornando o código mais eficiente.

Também é possível importar várias funções:

from func import somar, multiplicar
🔹 Pacotes (Packages)
Um pacote é uma pasta que agrupa módulos.
Para o Python reconhecer essa pasta como pacote, ela precisa conter um arquivo especial chamado __init__.py.

📌 Estrutura de Pacote

items/
 ├── __init__.py   # Torna a pasta um pacote
 ├── cadastro.py   # Módulo dentro do pacote
📥 Importando de um pacote

from items.cadastro import cliente, nova_funcao

cliente()
nova_funcao()
💡 Boas práticas
Não coloque todas as funções em um único arquivo.

Agrupe funções semelhantes no mesmo módulo.

Use pacotes para organizar projetos grandes.

Nomeie arquivos e funções de forma clara.
