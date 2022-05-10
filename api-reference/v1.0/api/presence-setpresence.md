---
title: 'presença: setPresence'
description: Defina as informações de presença para a sessão de presença do aplicativo de um usuário.
author: jsandoval-msft
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: c65754ffa61f62577ce4023d9a4a6e48ce0d533e
ms.sourcegitcommit: a11c874a7806fb5825752c8348e12079d23323e4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2022
ms.locfileid: "65293953"
---
# <a name="presence-setpresence"></a>presença: setPresence

Namespace: microsoft.graph

Defina o estado da sessão de presença de um usuário como um aplicativo.

### <a name="presence-sessions"></a>Sessões de presença
Um usuário pode ter várias sessões de presença porque o usuário pode estar em vários Teams clientes (desktop, móvel e Web). Cada Teams cliente tem uma sessão de presença independente e a presença do usuário é um estado agregado de todas as sessões por trás.

Da mesma forma, um aplicativo pode ter sua própria sessão de presença para um usuário e ser capaz de atualizar o estado.

Veja a seguir a precedência de como os estados de sessão são agregados:
* Configuração do > configurada pelo usuário (o estado configurado pelo usuário substitui outros)
* Entre os aplicativos configurados: DoNotDisturb (atualmente sem suporte para presença definida) > Ocupado > Disponível > Ausente

### <a name="timeout-expiration-and-keep-alive"></a>Tempo limite, expiração e manter-se ativo
Uma sessão **de presença pode** expirar **e expirar**, portanto, o aplicativo precisa chamar essa API antes do tempo **limite, para** manter o estado da sessão; ou antes da **expiração**, para manter a sessão ativa.

Uma sessão de presença poderá expirar se a disponibilidade for `Available` e o tempo limite for de 5 minutos. Quando atinge o tempo limite, o estado de presença esmaece em estágios. Por exemplo, se `Available/Available`um aplicativo definir a sessão de presença como , `Available/AvailableInactive` o estado será alterado para em 5 minutos com o primeiro tempo limite e, em seguida, `Away/Away` em mais 5 minutos com o segundo tempo limite.

A expiração de uma sessão de presença é configurável com o `expirationDuration` parâmetro. Quando uma sessão expira, ela se torna `Offline`.

## <a name="permissions"></a>Permissões
A permissão a seguir é necessária para chamar a API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Presence.ReadWrite                              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Application                            | Presence.ReadWrite.All                      |

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
| Sessionid          | string   | A ID da sessão de presença do aplicativo.                                                          |
| availability       | string   | As informações de presença base.                                                                         |
| atividade           | string   | As informações complementares à disponibilidade.                                                          |
| expirationDuration | duração | A expiração da sessão de presença do aplicativo. O valor é representado no formato ISO 8601 por durações.</p>Se não for fornecido, uma expiração padrão de 5 minutos será aplicada. O intervalo de duração válido é de 5 a 240 minutos (PT5M a PT4H)|

> [!IMPORTANT]
>
> Forneça a ID do aplicativo como `sessionId` na solicitação.

Combinações com suporte de `availability` e `activity` são:

| availability | atividade          | Descrição                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| Disponível    | Disponível         | Atualiza a sessão de presença como Disponível.               |
| Ocupado         | InACall           | Atualiza a sessão de presença como Ocupado, InACall.           |
| Ocupado         | InAConferenceCall | Atualiza a sessão de presença como Busy, InAConferenceCall. |
| Longe         | Longe              | Atualiza a sessão de presença como Ausente.                    |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK`.

## <a name="examples"></a>Exemplos
A solicitação a seguir mostra o aplicativo com a ID `22553876-f5ab-4529-bffb-cfe50aa89f87` que define sua sessão de presença para o usuário `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.

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

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/set-presence-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/set-presence-powershell-snippets.md)]
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
