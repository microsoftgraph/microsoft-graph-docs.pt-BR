---
title: 'openShiftChangeRequest: aprovar'
description: Aprovar uma solicitação openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3b6adfeb7cd69ba90b79aea5c1ec3108c3fd6085
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292396"
---
# <a name="openshiftchangerequest-approve"></a>openShiftChangeRequest: aprovar

Namespace: microsoft.graph

Aprovar um [objeto openShiftChangeRequest.](../resources/openshiftchangerequest.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Schedule.ReadWrite.All, Group.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Schedule.ReadWrite.All |

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais podem acessar grupos dos que não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|mensagem|String|Uma mensagem de aprovação personalizada.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

