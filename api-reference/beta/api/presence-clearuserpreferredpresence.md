---
title: 'presença: clearUserPreferredPresence'
description: Limpar a presença preferencial do usuário para um usuário
author: mkhribech
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 0fc72e76c9edb8d2104e720941b79c0e6dc67e9c
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391120"
---
# <a name="presence-clearuserpreferredpresence"></a>presença: clearUserPreferredPresence

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Limpe o status de disponibilidade e atividade preferencial para um usuário.

## <a name="permissions"></a>Permissões
A permissão a seguir é necessária para chamar a API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Presence.ReadWrite                          |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearUserPreferredPresence
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Essa solicitação contém apenas um objeto vazio.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK`.

## <a name="examples"></a>Exemplos

A solicitação a seguir limpa a presença preferencial do usuário para o usuário `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` .

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clearUserPreferredPresence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearUserPreferredPresence
Content-Type: application/json

{
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
