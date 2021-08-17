---
title: Obter appManagementPolicy
description: Obter uma política de gerenciamento de aplicativos.
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f1624b3c66746a0031cdf1878250dd72a5061524
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259017"
---
# <a name="get-appmanagementpolicy"></a>Obter appManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades de um [objeto appManagementPolicy.](../resources/appManagementPolicy.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                |
| :------------------------------------- | :--------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                             |
| Aplicativo                            | Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /policies/appManagementPolicies/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` único [objeto appManagementPolicy](../resources/appManagementPolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.  A partir da resposta, a política de gerenciamento de aplicativos define as seguintes restrições para objetos de entidade de serviço e aplicativo:

- Bloqueia a criação de novas senhas após 2019-10-19 às 10:37 hora UTC.
- Limita os segredos de senha para aplicativos criados após 2019-10-19 às 10:37 HORA UTC para menos de 4 dias, 12 horas, 30 minutos e 5 segundos.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appManagementPolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appmanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appmanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appmanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appmanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
  "description": "get appManagementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
