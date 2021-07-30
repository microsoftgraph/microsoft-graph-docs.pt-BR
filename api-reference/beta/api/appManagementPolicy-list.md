---
title: Listar appManagementPolicies
description: Obter uma lista de políticas de gerenciamento de aplicativos.
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c3a71c43f95c3aaef812f7c0b96917fa1928f542
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660352"
---
# <a name="list-appmanagementpolicies"></a>Listar appManagementPolicies

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [objetos appManagementPolicy.](../resources/appManagementPolicy.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                |
| :------------------------------------- | :--------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                             |
| Aplicativo                            | Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte `$select` aos `$filter` parâmetros de consulta , e OData para ajudar a personalizar `$top` a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /policies/appManagementPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objeto appManagementPolicy](../resources/appManagementPolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "list_appManagementPolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/appManagementPolicies
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/appManagementPolicies",
   "value": [
      {
         "id": "db9d4b58-3488-4da4-9994-49773c454e33",
         "displayName": "Custom app management policy",
         "description": "Custom policy that enforces app management restrictions on specific applications and service principals.",
         "isEnabled": false,
         "restrictions": {
            "passwordCredentials": [
               {
                  "restrictionType": "passwordAddition",
                  "maxLifetime": null,
                  "restrictForAppsCreatedAfterDateTime": "2019-10-19T10:37:00Z"
               },
               {
                  "restrictionType": "passwordLifetime",
                  "maxLifetime": "P4DT12H30M5S",
                  "restrictForAppsCreatedAfterDateTime": "2017-10-19T10:37:00Z"
               }
            ]
         }
      }
   ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "get appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
