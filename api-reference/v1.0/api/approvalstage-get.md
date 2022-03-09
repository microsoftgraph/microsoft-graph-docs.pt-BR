---
title: Obter approvalStage
description: Recupere as propriedades de um objeto approvalStage.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8f36fec1fa5ddafea069a168b7f3a1c07411406f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63398069"
---
# <a name="get-approvalstage"></a>Obter approvalStage

Namespace: microsoft.graph

No [gerenciamento de direitos do Azure AD](../resources/entitlementmanagement-overview.md), recupere as propriedades de um [objeto approvalStage](../resources/approvalstage.md) . Um estágio de aprovação está contido em um [objeto de](../resources/approval.md) aprovação.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{accessPackageAssignmentRequestId}/stages/{approvalStageId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e o [objeto approvalStage](../resources/approvalstage.md) no corpo da resposta. Se o chamador não tiver as permissões certas, o método retornará um `403 Forbidden` código de resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_approvalstage"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/stages/d4fa4045-4716-436d-aec5-57b0a713f095
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d4fa4045-4716-436d-aec5-57b0a713f095",
    "displayName": null,
    "reviewedDateTime": null,
    "reviewResult": "NotReviewed",
    "status": "InProgress",
    "assignedToMe": true,
    "justification": "",
    "reviewedBy": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approvalStage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


