---
title: Clonar uma equipe
description: Crie uma cópia de uma equipe. Essa operação também cria uma cópia do grupo correspondente.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 17d2125299952a2a89ab3e86d4a66dee4aa9119c
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2022
ms.locfileid: "62442831"
---
# <a name="clone-a-team"></a>Clonar uma equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie uma cópia de uma [equipe](../resources/team.md). Essa operação também cria uma cópia do grupo [correspondente](../resources/group.md).
Você pode especificar quais partes da equipe clonar:

- **apps** - copia Microsoft Teams aplicativos instalados na equipe. 
- **canais** – Copia a estrutura do canal (mas não as mensagens no canal).
- **membros** – Copia os membros e proprietários do grupo.
- **configurações** – Copia todas as configurações dentro da equipe, juntamente com as principais configurações de grupo.
- **guias** – Copia as guias dentro dos canais.

Quando as guias são clonadas, elas são colocadas em um estado não configurado - elas são exibidas na barra de guias no Microsoft Teams e, na primeira vez que você abri-las, você vai passar pela tela de configuração. (Se a pessoa que abre a guia não tiver permissão para configurar aplicativos, ela verá uma mensagem explicando que a guia não foi configurada.)

A clonagem é uma operação de longa duração.
Depois que o clone POST retorna, você precisa OBTER a [](../resources/teamsasyncoperation.md) operação retornada pelo header Location: para ver se ele está "em execução" ou "bem-sucedido" ou "falhou". Você deve continuar a OBTER até que o status não seja "em execução". O atraso recomendado entre GETs é de 5 segundos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Team.Create, Group.ReadWrite.All **, Directory.ReadWrite.All** |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo                            | Team.Create, Group.ReadWrite.All **, Directory.ReadWrite.All** |

> **Observação**: As permissões marcadas com ** só têm suporte para compatibilidade com compatibilidade Recomendamos que você atualize suas soluções para usar permissões diferentes e evite usar essas permissões adiante.

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
|classificação|Cadeia de caracteres (opcional)|Descreve uma classificação para o grupo (como baixo, médio ou alto impacto comercial). Os valores válidos para essa propriedade são definidos criando um valor de configuração [ClassificationList,](../resources/directorysetting.md) com base na [definição do modelo](../resources/directorysettingtemplate.md). Se a classificação não for especificada, a classificação será copiada da equipe/grupo original.|
|description|Cadeia de caracteres (opcional)|Uma descrição opcional para o grupo. Se essa propriedade não for especificada, ela ficará em branco.|
|displayName|String|O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|mailNickname|String|O alias de email do grupo, exclusivo na organização. Essa propriedade deve ser especificada quando um grupo é criado. Oferece suporte a $filter. Se essa propriedade não for especificada, ela será calculada a partir do displayName. Problema conhecido: essa propriedade é ignorada no momento.|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |Uma lista separada por vírgulas das partes a ser clonada. As partes legais são "aplicativos, guias, configurações, canais, membros".|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)| Especifica a visibilidade do grupo. Os valores possíveis são: **Privado**, **Público**. Se a visibilidade não for especificada, a visibilidade será copiada da equipe/grupo original. Se a equipe que está sendo clonada for uma equipe **educationClass** , o parâmetro de visibilidade será ignorado e a visibilidade do novo grupo será definida como HiddenMembership.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `202 Accepted` código de resposta com um header Location: apontando para o recurso [de](../resources/teamsasyncoperation.md) operação.
Quando a operação for concluída, o recurso de operação dirá a id da equipe criada.

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

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/clone-team-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/clone-team-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Eis um exemplo da resposta. Observação: o objeto de resposta exibido aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


