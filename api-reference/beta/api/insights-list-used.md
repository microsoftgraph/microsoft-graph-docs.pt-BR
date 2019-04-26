---
title: Listar usados
description: Informações calculadas que retornam a lista de arquivos usados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 053f36b893cf2167cd30ea8ca1fe639a6df22494
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328647"
---
# <a name="list-used"></a>Listar usados

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações calculadas que retornam a lista de arquivos usados com um usuário.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
```http
GET /me/insights/used
```
Solicitar que os documentos usados de outros usuários retornem resultados classificados por "lastModifiedDateTime" e "lastAccessedDateTime" está definido como "lastModifiedDateTime".
```http
GET /users/{id | userPrincipalName}/insights/used
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

Você pode usar o `$filter` parâmetro de consulta para filtrar itens usados. Por exemplo, com base no tipo:

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Ou com base no tipo de contêiner:

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

ConFira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       |  Valor|
|:-------------|:------|
| Autorização  | {token} de portador. Obrigatório.|
| Aceitar  | application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens [usados](../resources/insights-used.md) no corpo da resposta.
## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real. 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```

### <a name="expanding-resource"></a>Expandindo recurso
O recurso mencionado por uma visão usada pode ser expandido.
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
