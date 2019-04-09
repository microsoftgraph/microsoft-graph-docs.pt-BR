---
title: Ignorar riskyUsers
description: DesCartar o risco de um objeto riskyUsers.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 3027320b25c35e60e1b5dccabc7ff34ea642a953
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2019
ms.locfileid: "31560098"
---
# <a name="dismiss-riskyusers"></a>Ignorar riskyUsers

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.

DesCartar o risco de um objeto **riskyUser** . Esta ação definirá o nível de risco do usuário de destino como nenhum.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Identityriskuser. ReadWrite. All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Identityriskuser. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Workbook-Session-Id  | ID da sessão da pasta de trabalho que determina se as alterações são persistentes. Opcional.|

## <a name="request-body"></a>Corpo da solicitação
Especifique as userIds a serem descartadas no corpo da solicitação.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
