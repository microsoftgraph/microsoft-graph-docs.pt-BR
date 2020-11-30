---
title: Criar permissionGrantPolicy
description: Cria um objeto permissionGrantPolicy que descreve as condições sob as quais as permissões podem ser concedidas.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 3cfd4a0b13ff3e65be5ffdc8e3486343bef9ce2c
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377115"
---
# <a name="create-permissiongrantpolicy"></a>Criar permissionGrantPolicy

Namespace: microsoft.graph

Cria um [permissionGrantPolicy](../resources/permissiongrantpolicy.md). Uma política de concessão de permissão é usada para descrever as condições sob as quais podem ser concedidas permissões (por exemplo, durante o consentimento do aplicativo).

Após criar a política de concessão de permissão, você pode [Adicionar conjuntos de condições de inclusão](permissiongrantpolicy-post-includes.md) para adicionar regras de correspondência e [Adicionar conjuntos de condições](permissiongrantpolicy-post-excludes.md) de exclusão para adicionar regras de exclusão.

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
POST /policies/permissionGrantPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [permissionGrantPolicy](../resources/permissiongrantpolicy.md) .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [permissionGrantPolicy](../resources/permissiongrantpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "create_permissiongrantpolicy"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies
Content-Type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
