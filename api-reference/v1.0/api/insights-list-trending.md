---
title: Listar tendências
description: Insights calculados que retornam a lista de itens de tendências do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 604a05ab01312707b52274c6276ce044349f0d43
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473189"
---
# <a name="list-trending"></a>Listar tendências

Namespace: microsoft.graph

Insights calculados que incluem uma lista de documentos que são tendências ao redor do usuário.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
Obter uma lista de documentos que são tendências em torno do usuário ou usuário especificado:

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

Expanda o recurso referenciado por **uma visão de tendência:**

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

Você pode usar o `$filter` parâmetro de consulta para filtrar itens de tendência. Por exemplo, com base no **tipo**:

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

Ou com base em **containerType**:

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

Consulte os tipos e tipos de contêiner disponíveis que você pode filtrar em [resourceVisualization](../resources/insights-resourcevisualization.md).


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       |  Valor|
|:-------------|:------|
| Autorização  | {token} de portador. Obrigatório.|
| Aceitar  | application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma lista de itens `200 OK` [de](../resources/insights-trending.md) tendência no corpo da resposta. Cada item contém propriedades de visualização para exibir o item em sua experiência.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real. Consulte um exemplo de resposta não truncada na parte inferior da página.
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "AWMiSOpKHlJCpP_ZoVJQXi9ees4wFhDQQqF55Pm5DlaMzvtd2zra4UWSTEvpTldvb6EhQ289G4BAsxnrajQyjW1jIkjqSh5SQqT_2aFSUF4vBQ",
            "weight": "0.1583399742569597",
            "resourceVisualization": {
                "title": "LiveCaptions",
                "type": "Image",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerWebUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared Documents/Go to Market Plan",
                "containerDisplayName": "Mark 8 Project Team",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared%20Documents/Go%20to%20Market%20Plan/LiveCaptions.gif",
                "id": "drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```
