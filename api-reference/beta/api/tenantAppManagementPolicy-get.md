---
title: Obter tenantAppManagementPolicy
description: Leia a política de locatário padrão que se aplica a aplicativos e objetos de entidades de serviço.
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1d9acdcb2f98713de5be40333ddc627678fa3fa9
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660361"
---
# <a name="get-tenantappmanagementpolicy"></a>Obter tenantAppManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades de um [objeto tenantAppManagementPolicy.](../resources/tenantAppManagementPolicy.md)

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
GET /policies/tenantAppManagementPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [tenantAppManagementPolicy](../resources/tenantAppManagementPolicy.md) solicitado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_tenantAppManagementPolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tenantAppManagementPolicy
```

### <a name="response"></a>Resposta

A seguir, um exemplo da resposta que mostra a política de gerenciamento de aplicativos de locatário padrão.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tenantAppManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/tenantAppManagementPolicy/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/defaultAppManagementPolicy/00000000-0000-0000-0000-000000000000",
    "id": "00000000-0000-0000-0000-000000000000",
    "displayName": "Default app management tenant policy",
    "description": "Default tenant policy that enforces app management restrictions on applications and service principals. To apply policy to targeted resources, create a new policy under appManagementPolicies collection.",
    "isEnabled": false,
    "applicationRestrictions": {
        "passwordCredentials": []
    },
    "servicePrincipalRestrictions": {
        "passwordCredentials": []
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tenantAppManagementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
