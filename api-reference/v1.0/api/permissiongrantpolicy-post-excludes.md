---
title: Criar permissionGrantConditionSet na coleção Excludes de permissionGrantPolicy
description: Adicionar condições sob as quais um evento de concessão de permissão é excluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9011d194e0de5f0efea0d5a483219896b0f71073
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377121"
---
# <a name="create-permissiongrantconditionset-in-excludes-collection-of-permissiongrantpolicy"></a>Criar permissionGrantConditionSet na coleção Excludes de permissionGrantPolicy

Namespace: microsoft.graph

Adicionar condições sob as quais um evento de concessão de permissão é *excluído* em uma política de concessão de permissão. Para fazer isso, adicione um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) à coleção **Excludes** de um  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Policy.ReadWrite.PermissionGrant |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | Policy.ReadWrite.PermissionGrant |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Neste exemplo, *todas* as permissões delegadas para o Microsoft Graph (**AppID** 00000003-0000-0000-C000-000000000000) são excluídas da política de concessão de permissão.

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_excludes"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/excludes
Content-Type: application/json

{
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "9a532f49-e646-405d-8c7c-d4c8e8a4d294",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
