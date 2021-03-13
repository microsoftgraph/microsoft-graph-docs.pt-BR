---
title: Atualizar approvalStep
description: Aplicar aprovar ou negar decisão em um objeto approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 16c2796e94678b4ca0362c3be86268f69cdbcedb
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760746"
---
# <a name="update-approvalstep"></a>Atualizar approvalStep

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aplicar aprovar ou negar decisão em um [objeto approvalStep.](../resources/approvalStep.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

A tabela a seguir mostra as propriedades necessárias para este método.

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
| reviewResult | String | Decisão do aprovador. Os valores possíveis são: `Approve` e `Deny`.|
| justification | String | Justificativa relacionada à decisão do aprovador. |


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `204 No Content` um código de resposta no corpo da resposta. No entanto, se o chamador não tiver as permissões certas, o método retornará um código de resposta ou se a id de aprovação não for encontrada, o `403 Forbidden` método retornará `404 Not found` . Se a solicitação já tiver sido aprovada por outro aprovador no mesmo estágio de aprovação, o método `409 Conflict` retornará no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "patch_approvalstep"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-Type: application/json
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
