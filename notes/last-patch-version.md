# Usar o til para usar sempre a última versão de patch de uma dependência

No último desafio, você disse ao npm para incluir apenas uma versão específica de um pacote. Essa é uma maneira útil de congelar suas dependências, caso você precise garantir que diferentes partes do seu projeto permaneçam compatíveis entre si. Mas, na maioria dos casos de uso, você não quer perder as correções de erros, já que elas geralmente incluem correções de segurança importantes e (esperamos que) não quebrem nada ao fazer isso.

Para permitir que uma dependência do npm atualize para a última versão de PATCH, você pode prefixar a versão da dependência com o caractere de til `(~)`. Aqui está um exemplo de como permitir atualizações para qualquer versão 1.3.x

~~~json
"package": "~1.3.8"
~~~