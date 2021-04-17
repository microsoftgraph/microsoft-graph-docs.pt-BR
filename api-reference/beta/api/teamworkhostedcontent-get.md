---
title: Obter o trabalho em equipeHostedContent
description: Recupere o conteúdo hospedado em um teamsAppIcon.
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b5fde96ffaad34360603751398473357d82e1fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882634"
---
# <a name="get-teamworkhostedcontent"></a>Obter o trabalho em equipeHostedContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere o [conteúdo hospedado](../resources/teamworkhostedcontent.md) no ícone de [um aplicativo.](../resources/teamsappicon.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-for-app-icon-in-app-catalog"></a>Permissões para ícone de aplicativo no catálogo de aplicativos
| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                   |
| Aplicativo                            | Sem suporte.                                                   |

## <a name="http-request"></a>Solicitação HTTP

**Obter conteúdo hospedado no ícone do aplicativo no catálogo de aplicativos**

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/$value
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/$value
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Essa operação dá suporte aos `$select` [parâmetros de consulta OData](/graph/query-parameter) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho           | Valor                      |
| :--------------- | :------------------------- |
| Autorização    | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [teamworkHostedContent](../resources/teamworkhostedcontent.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-bytes-of-the-hosted-content-of-the-color-icon-of-a-teams-app-in-the-catalog"></a>Exemplo 1: Obter os bytes do conteúdo hospedado do ícone de cor de um aplicativo do Teams no catálogo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontent_coloricon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/
```


#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

> **Observação:** `contentBytes` e `contentType` são sempre definidos como nulos.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/hostedContent/$entity",
    "id": "aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-the-bytes-of-the-hosted-content-of-the-outline-icon-of-a-teams-app-in-the-catalog"></a>Exemplo 2: Obter os bytes do conteúdo hospedado do ícone de contorno de um aplicativo do Teams no catálogo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

> **Observação:** As solicitações para o valor bruto não suportam [parâmetros de](/graph/query-parameters) consulta OData para personalizar a resposta.

<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontentbytes_outlineicon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value
```

#### <a name="response"></a>Resposta

A resposta contém bytes para o conteúdo hospedado no corpo. `content-type` o header especifica o tipo de conteúdo hospedado.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/png
```

## <a name="see-also"></a>Confira também

- [Obter ícones de um aplicativo do Teams](teamsappicon-get.md)
- [Listar aplicativos no catálogo](appcatalogs-list-teamsapps.md)
