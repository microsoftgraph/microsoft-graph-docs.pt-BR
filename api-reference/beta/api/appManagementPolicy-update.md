---
title: Atualizar appManagementPolicy
description: Atualize uma política de gerenciamento de aplicativos.
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7682aff0026b94e4b3f68bd173c8d582ec212ff3
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660336"
---
# <a name="update-appmanagementpolicy"></a>Atualizar appManagementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize [um objeto appManagementPolicy.](../resources/appManagementPolicy.md)

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
PATCH /policies/appManagementPolicies/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece os valores para campos relevantes do [appManagementPolicy](../resources/appManagementPolicy.md) que devem ser atualizados.
Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.
Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade                | Tipo                                                                        | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|:------------------------|:----------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName  | Cadeia de caracteres                                                      | O nome de exibição da política. Herdado de [policyBase](../resources/policybase.md).                                        |
| description  | Cadeia de caracteres                                                      | A descrição da política. Herdado de [policyBase](../resources/policybase.md).                                         |
| isEnabled    | Booliano                                                     | Indica se a política está habilitada.                                      |
| restrictions | [appManagementConfiguration](../resources/appManagementConfiguration.md) | Restrições que se aplicam a um objeto de entidade de serviço ou aplicativo. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_appManagementPolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}

{
    "isEnabled": false
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
  "description": "update appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
