---
title: Criar tokenLifetimePolicy
description: Criar um novo tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d40146e205dd250f99df3334b5e0c8d0323564c7
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234112"
---
# <a name="create-tokenlifetimepolicy"></a>Criar tokenLifetimePolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Policy. ReadWrite. ApplicationConfiguration |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Policy. ReadWrite. ApplicationConfiguration |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {token} |
| Content-type | application/json |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->