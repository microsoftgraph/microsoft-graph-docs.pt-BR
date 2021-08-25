---
title: 'presença: setPresence'
description: De definir as informações de presença para a sessão de presença do aplicativo do usuário.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 71ee6d63f2dfc8664705412c0bc257959094040e
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514018"
---
# <a name="presence-setpresence"></a>presença: setPresence

Namespace: microsoft.graph

De definir o estado da sessão de presença de um usuário como um aplicativo.

### <a name="presence-sessions"></a>Sessões de presença
Um usuário pode ter várias sessões de presença porque o usuário pode estar em vários Teams clientes (desktop, móvel e Web). Cada Teams cliente tem uma sessão de presença independente e a presença do usuário é um estado agregado de todas as sessões atrás.

Da mesma forma, um aplicativo pode ter sua própria sessão de presença para um usuário e ser capaz de atualizar o estado.

Veja a seguir a precedência de como os estados de sessão são agregados:
* Configurada pelo usuário > configurada pelo aplicativo (o estado configurado pelo usuário substitui outras pessoas)
* Entre os aplicativos configurados: DoNotDisturb (atualmente sem suporte para a presença definida) > Ocupado > Disponível > Distância

### <a name="timeout-expiration-and-keep-alive"></a>Tempo de expiração, expiração e manter-se vivo
Uma sessão de presença pode **expirar** e **expirar**, portanto, o aplicativo precisa chamar essa API antes do tempo de tempo, para manter o estado da sessão; ou antes da **expiração**, para manter a sessão viva.

Uma sessão de presença pode ser limitada se a disponibilidade for `Available` e o tempo-de-tempo for de 5 minutos. Quando o tempo passa, o estado de presença desaparece em estágios. Por exemplo, se um aplicativo define a sessão de presença como , o estado será alternado para em 5 minutos com o primeiro tempo de tempo, em seguida, em outros 5 minutos com o `Available/Available` `Available/AvailableInactive` segundo `Away/Away` tempo.

A expiração de uma sessão de presença é configurável com o `expirationDuration` parâmetro. Quando uma sessão expira, ela se torna `Offline` .

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
POST /users/{userId}/presence/setPresence
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro          | Tipo     | Descrição                                                                                            |
| :----------------- | :------- | :----------------------------------------------------------------------------------------------------- |
| sessionId          | cadeia de caracteres   | A ID da sessão de presença do aplicativo.                                                          |
| availability       | cadeia de caracteres   | As informações de presença base.                                                                         |
| atividade           | cadeia de caracteres   | As informações complementares à disponibilidade.                                                          |
| expirationDuration | duração | A expiração da sessão de presença do aplicativo. O valor é representado no formato ISO 8601 por durações.</p>Se não for fornecido, será aplicada uma expiração padrão de 5 minutos. |

> [!IMPORTANT]
>
> Forneça a ID do aplicativo como `sessionId` na solicitação.

Combinações com suporte de `availability` e `activity` são:

| availability | atividade          | Descrição                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| Disponível    | Disponível         | Atualiza a sessão de presença como Disponível.               |
| Ocupado         | InACall           | Atualiza a sessão de presença como Ocupado, InACall.           |
| Ocupado         | InAConferenceCall | Atualiza a sessão de presença como Busy, InAConferenceCall. |
| Away         | Away              | Atualiza a sessão de presença como Distante.                    |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK`.

## <a name="examples"></a>Exemplos
A solicitação a seguir mostra o aplicativo com ID `22553876-f5ab-4529-bffb-cfe50aa89f87` que define sua sessão de presença para o usuário `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` .

### <a name="request"></a>Solicitação



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "set-presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87",
  "availability": "Available",
  "activity": "Available",
  "expirationDuration": "PT1H"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/set-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/set-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/set-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/set-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
