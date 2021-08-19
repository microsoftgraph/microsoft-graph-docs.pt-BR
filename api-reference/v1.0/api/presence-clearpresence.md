---
title: 'presença: clearPresence'
description: Desmarcar as informações de presença para a sessão de presença do aplicativo do usuário.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 02140f99accf36bfac156996e83bd75de2bb3b19
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58397079"
---
# <a name="presence-clearpresence"></a>presença: clearPresence

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Desmarcar a sessão de presença do aplicativo para um usuário. Se for a única sessão de presença do usuário, a presença do usuário mudará para `Offline/Offline` .

Para obter detalhes sobre sessões de presença, [consulte presence: setPresence](presence-setpresence.md#presence-sessions).

## <a name="permissions"></a>Permissões
A permissão a seguir é necessária para chamar a API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Sem suporte.                              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearPresence
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo   | Descrição                                   |
| :-------- | :----- | :-------------------------------------------- |
| sessionId | string | A ID da sessão de presença do aplicativo. |


> [!IMPORTANT]
> 
> Forneça a ID do aplicativo como `sessionId` na solicitação.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK`.

Se a sessão de presença não existir, este método retornará um `404 NotFound` código de resposta.

## <a name="examples"></a>Exemplos
A solicitação a seguir mostra o aplicativo com ID `22553876-f5ab-4529-bffb-cfe50aa89f87` que limpa sua sessão de presença para o usuário `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` .

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "clear--presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87"
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
