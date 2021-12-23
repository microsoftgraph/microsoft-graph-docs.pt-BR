---
title: 'presença: setUserPreferredPresence'
description: Definir a presença preferencial do usuário para um usuário
author: mkhribech
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 005c0c6cd0f35455780c11650a10bab96280bc6d
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526083"
---
# <a name="presence-setuserpreferredpresence"></a>presença: setUserPreferredPresence

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

De definir o status de disponibilidade e atividade preferencial para um usuário. Se a presença preferencial de um usuário estiver definida, a presença do usuário será a presença preferencial.

A presença preferencial só entra em vigor quando há pelo menos uma sessão [de presença](presence-setpresence.md#presence-sessions) do usuário. Caso contrário, a presença do usuário permanece offline.

Uma sessão de presença pode ser criada como resultado de uma operação [setPresence](presence-setpresence.md) bem-sucedida ou se o usuário estiver Teams cliente. 

Leia mais sobre [sessões de presença](presence-setpresence.md#presence-sessions) e seu [tempo de expiração e expiração.](presence-setpresence.md#timeout-expiration-and-keep-alive) 

## <a name="permissions"></a>Permissions
A permissão a seguir é necessária para chamar a API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Presence.ReadWrite                          |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/setUserPreferredPresence
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro          | Tipo     | Descrição                                                                                                                                                                                                                                    |
| :----------------- | :------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| availability       | string   | As informações de presença base.                                                                                                                                                                                                                 |
| atividade           | string   | As informações complementares à disponibilidade.                                                                                                                                                                                                  |
| expirationDuration | duração | A expiração da sessão de presença do aplicativo. O valor é representado no formato ISO 8601 por durações.<br/>Se não for fornecido, será aplicada uma expiração padrão:<br/>DoNotDisturb ou Ocupado: expira em 1 dia<br/>Todos os outros: expira em 7 dias |

As combinações de **disponibilidade** e atividade com suporte **são:**

| availability | atividade     | Descrição                                         |
| :----------- | :----------- | :-------------------------------------------------- |
| Disponível    | Disponível    | De definir a presença preferencial do usuário como Disponível.       |
| Ocupado         | Ocupado         | De definir a presença preferencial do usuário como Ocupado.            |
| DoNotDisturb | DoNotDisturb | De definir a presença preferencial do usuário como DoNotDisturb.    |
| BeRightBack  | BeRightBack  | De definir a presença preferencial do usuário como BeRightBack.     |
| Away         | Away         | De definir a presença preferencial do usuário como Away.            |
| Offline      | OffWork      | De definir a presença preferencial do usuário como Offline. |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK`.

## <a name="examples"></a>Exemplos

A solicitação a seguir define a presença preferencial do usuário como DoNotDisturb para o usuário , com a `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` expiração de 8 horas.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "setUserPreferredPresence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setUserPreferredPresence
Content-Type: application/json

{
  "availability": "DoNotDisturb",
  "activity": "DoNotDisturb",
  "expirationDuration": "PT8H"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/setuserpreferredpresence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/setuserpreferredpresence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/setuserpreferredpresence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/setuserpreferredpresence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/setuserpreferredpresence-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
