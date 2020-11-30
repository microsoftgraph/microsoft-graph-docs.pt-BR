---
title: Criar permissionGrantConditionSet na coleção de inclusões de permissionGrantPolicy
description: Adicionar condições sob as quais um evento de concessão de permissão é incluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 42778a7eaae409a9d8602a1c9faf1189de446f79
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377143"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a>Criar permissionGrantConditionSet na coleção de inclusões de permissionGrantPolicy

Namespace: microsoft.graph

Adicionar condições sob as quais um evento de concessão de permissão é *incluído* em uma política de concessão de permissão. Para fazer isso, adicione um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) à coleção de **inclusões** de um  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).

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
POST /policies/permissionGrantPolicies/{id}/includes
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

Neste exemplo, *todas* as permissões delegadas para aplicativos clientes de editores verificados estão incluídas na política de concessão de permissão. Como todas as outras condições do [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) foram omitidas, elas terão seus valores padrão, o que, em cada caso, é o mais inclusivo.

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_includes"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/{id}/includes
Content-Type: application/json

{
  "permissionType": "delegated",
  "clientApplicationsFromVerifiedPublisherOnly": true
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
  "id": "75ffda85-9314-43bc-bf19-554a7d079e96",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "any",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
