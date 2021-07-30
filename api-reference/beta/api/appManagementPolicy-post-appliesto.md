---
title: Atribuir appliesTo
description: Atribua uma política ao objeto de entidade de serviço ou aplicativo.
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6bcc15108d43fc82c3ac643e18bb48e043291841
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660339"
---
# <a name="assign-appliesto"></a>Atribuir appliesTo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atribua um [objeto de política appManagementPolicy](../resources/appManagementPolicy.md) a um objeto de entidade de serviço ou aplicativo. A entidade de serviço ou aplicativo adota essa política na configuração [tenantAppManagementPolicy](../resources/tenantappmanagementpolicy.md) em todo o locatário. Somente um objeto de política pode ser atribuído a um aplicativo ou entidade de serviço.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                |
| :------------------------------------- | :--------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Policy.ReadWrite.ApplicationConfiguration |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                             |
| Aplicativo                            | Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/appManagementPolicies/$ref
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma referência a um único objeto de política da [coleção appManagementPolicies.](../resources/appmanagementpolicy.md)

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

A seguir, um exemplo da solicitação para atribuir um appManagementPolicy a um aplicativo.

<!-- {
  "blockType": "request",
  "name": "assign_appliesTo"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applications/{id}/appManagementPolicies/$ref

{
 "@odata.id":"https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "list resources for appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
