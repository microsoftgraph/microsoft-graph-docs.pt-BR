---
title: Clonar uma equipe
description: Criar uma cópia de uma equipe. Essa operação também cria uma cópia do grupo correspondente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5368e2128a5c4010f218639574104a09371636ee
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335688"
---
# <a name="clone-a-team"></a>Clonar uma equipe

Namespace: microsoft.graph



Criar uma cópia de uma [equipe](../resources/team.md). Essa operação também cria uma cópia do [grupo](../resources/group.md)correspondente.
Você pode especificar quais partes da equipe serão clonadas:

- **aplicativos** – copia os aplicativos do Microsoft Teams instalados na equipe. 
- **canais** – copia a estrutura do canal (mas não as mensagens no canal).
- **Membros** – copia os membros e os proprietários do grupo.
- **configurações** – copia Todas as configurações da equipe, juntamente com as configurações de grupo de chaves.
- **guias** – copia as guias nos canais.

Quando as guias são clonadas, elas são colocadas em um estado não configurado – elas são exibidas na barra de guias do Microsoft Teams e na primeira vez que você as abre, você passará pela tela de configuração. (Se a pessoa que estiver abrindo a guia não tiver permissão para configurar aplicativos, verá uma mensagem explicando que a guia não foi configurada.)

A clonagem é uma operação de execução demorada.
Após o cancelamento do clone da POSTAgem, você precisará obter a [operação](../resources/teamsasyncoperation.md) para ver se ela está "em execução" ou "com êxito" ou "falha". Você deve continuar a obter até que o status não seja "em execução". O atraso recomendado entre GETs é de 5 segundos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Group.ReadWrite.All, Directory.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo                            | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classificação|Cadeia de caracteres (opcional)|Descreve uma classificação para o grupo (como impacto comercial baixo, médio ou alto). Se a classificação não for especificada, a classificação será copiada da equipe/grupo original.|
|description|Cadeia de caracteres (opcional)|Uma descrição opcional para o grupo. Se essa propriedade não for especificada, será deixada em branco.|
|displayName|String|O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|mailNickname|String|O alias de email do grupo, exclusivo na organização. Essa propriedade deve ser especificada quando um grupo é criado. Oferece suporte a $filter. Se essa propriedade não for especificada, será calculada a partir do displayName. Problema conhecido: esta propriedade é ignorada no momento.|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |Uma lista separada por vírgulas das partes a serem clonadas. As partes legais são "aplicativos, guias, configurações, canais, membros".|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)| Especifica a visibilidade do grupo. Os valores possíveis são: **Private**, **Public**. Se a visibilidade não for especificada, a visibilidade será copiada da equipe/grupo original. Se a equipe que está sendo clonada for uma equipe do **educationClass** , o parâmetro Visibility será ignorado e a visibilidade do novo grupo será definida como HiddenMembership.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `202 Accepted` código de resposta com um local: cabeçalho apontando para o recurso [Operation](../resources/teamsasyncoperation.md) .
Quando a operação for concluída, o recurso de operação informará o ID da equipe criada.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clone_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clone-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clone-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clone-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clone-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta. Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
