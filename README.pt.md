# O que é um changelog?

Um changelog é um arquivo que contém uma lista *ordenada cronologicamente* das mudanças *notáveis* para cada versão de um projeto.

# Por que manter um changelog?

Para que seja mais fácil para as usuárias e colaboradoras verem exatamente quais mudanças notáveis foram feitas entre cada lançamento (ou versão) do projeto.

As usuárias do software, sejam consumidoras finais ou desenvolvedoras, são seres humanos que se preocupam com o que está no software. Quando o software muda, as pessoas querem saber o porquê, o que e como. Desta forma, o changelog ajuda as usuárias a decidirem se devem ou não atualizar para uma nova versão do software e ajuda as desenvolvedoras a rastrear as mudanças que foram feitas no software e facilita a resolução de problemas quando algo dá errado.

No caso particular do Bootcamp WebDev da Laboratoria, manter um changelog para cada projeto que você desenvolver tem os seguintes objetivos:
- Identificar os avanços sprint a sprint em seu projeto
- Identificar os aprendizados sprint a sprint em seu projeto
- Avaliar a qualidade e utilidade das mensagens de seus commits

# Que formato devo usar para o Changelog de um projeto da Laboratoria?

Em primeiro lugar, você deve criar um arquivo `CHANGELOG.md` na raiz do seu projeto.

Depois, ao terminar cada sprint, antes da cerimônia de _Sprint Review_, você deverá adicionar uma nova entrada no início do arquivo com os avanços e aprendizados da última sprint, usando o seguinte formato:

```md
## <versão> - <data>

### Aprendizados da Sprint

Nesta seção, liste os aprendizados da sprint.

### Adicionado

Nesta seção, especifique as funcionalidades que você adicionou.

### Alterado

Nesta seção, detalhe as alterações que você fez em funcionalidades já existentes.

### Corrigido

Nesta seção, descreva os _bugs_ corrigidos.

### Removido

Nesta seção, inclua as funcionalidades removidas.
```

No formato acima, você deve substituir `<versão>` pelo número da nova versão liberada, por exemplo, 1.0.1, e `<data>` pela data de liberação no formato AAAA-MM-DD, por exemplo, 2023-09-20.

O número da versão deve seguir o padrão do [Semantic Versioning](https://semver.org/), que estabelece que:

>Dado um número de versão MAIOR.MENOR.PATCHES, aumente o seguinte:
>
>    Versão MAIOR quando você faz alterações incompatíveis na API
>
>    Versão MENOR quando adiciona funcionalidade de forma compatível com versões anteriores
>
>    Versão PATCHES quando faz correções de bugs compatíveis com versões anteriores

# Consulta de commits na sprint

Você pode executar o seguinte comando para consultar as mensagens de commits que você fez nos últimos 7 dias em todas as branches do seu repositório e, assim, construir seu changelog:

``git log --all --since='7 days ago' --oneline --format="* %h %s (%an) %as"``

O resultado deste comando pode parecer como o seguinte:

>* 4a87adb refactor in request hook (Carlos Gonzalez) 2023-09-19
>* 388f431 README improvements (Sergio Sinuco) 2023-09-19
>* 509bcf8 Adjust readme with images and components description, adjusted some types and params (Kvn Alvarado) 2023-09-18

# Exemplo

No arquivo [EXAMPLE.pt.md](./EXAMPLE.pt.md), você encontrará um changelog de exemplo.
