# Usar o circunflexo para usar a última versão secundária de uma dependência

Da mesma forma que o til, que aprendemos no último desafio e que permite que o npm instale o último PATCH de uma dependência, o circunflexo (`^`) permite que o npm instale atualizações futuras também. A diferença é que o circunflexo permitirá tanto atualizações MINOR quanto PATCHes.

Sua versão atual de `@freecodecamp/example` deve ser "~1.2.13", o que permitirá que o npm instale a versão 1.2.x mais recente. Se você usasse o circunflexo (^) como um prefixo de versão, o npm teria permissão para atualizar para qualquer versão 1.x.x.

~~~json
"package": "^1.3.8"
~~~

Isso permitiria atualizações para qualquer versão 1.x.x do pacote.