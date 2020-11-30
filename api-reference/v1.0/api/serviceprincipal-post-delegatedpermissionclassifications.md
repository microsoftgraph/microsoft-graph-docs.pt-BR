---
title: Criar delegatedPermissionClassification
description: Classificar uma permissão adicionando um delegatedPermissionClassification à entidade de serviço da API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 22512ad7a61d528d22535156c1ac882b73950f72
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377140"
---
# <a name="create-delegatedpermissionclassification"></a>Criar delegatedPermissionClassification

Namespace: microsoft.graph

Classificar uma permissão delegada adicionando um [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) ao [servicePrincipalName](../resources/servicePrincipal.md) que representa a API.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | PermissionGrantPolicy. ReadWrite. All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | PermissionGrantPolicy. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

No exemplo a seguir, a permissão delegada "User. Read" está sendo classificada como "Low".

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "2G3-4TG6YU2J54hjnaRoPQE",
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
