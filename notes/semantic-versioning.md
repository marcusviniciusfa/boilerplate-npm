# Gerenciar dependências do npm entendendo o versionamento semântico

As `Versions` (versões) dos pacotes do npm na seção de dependências do seu arquivo package.json seguem o que chamamos de Semantic Versioning (SemVer), um padrão do setor para versionamento de software, com o objetivo de facilitar o gerenciamento de dependências. Bibliotecas, frameworks ou outras ferramentas publicadas no npm devem usar o SemVer para comunicar claramente que tipo de mudanças os projetos podem esperar caso eles atualizem.

Conhecer o SemVer pode ser útil quando você desenvolve um software que usa dependências externas (algo que você faz quase sempre). Um dia, seu entendimento desses números vai evitar que você introduza acidentalmente alterações que causem problemas em seu projeto, sem compreender por que as coisas que funcionaram ontem, de repente, não funcionam hoje. É assim que o Versionamento Semântico funciona de acordo com o site oficial:

~~~json
"package": "MAJOR.MINOR.PATCH"
~~~

A versão MAJOR (principal) deve incrementar quando você fizer alterações incompatíveis na API. A versão MINOR (secundária) deve incrementar quando adicionar funcionalidades retrocompatíveis. A versão PATCH deve incrementar quando você fizer consertos de bugs retrocompatíveis. Isso significa que PATCHes são correções de bugs e MINORs adicionam novas funcionalidades, mas nenhum deles quebra o que funcionava antes. Por fim, as MAJORs adicionam alterações que não funcionarão com versões anteriores.