---
title: Remover canal
description: Remova um canal de entrada.
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: aad792df2ed019893e3e1c735929fb053a1e3758
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628906"
---
# <a name="remove-channel"></a>Remover canal
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Remova um [canal](../resources/channel.md) de entrada (um **canal** compartilhado com uma **equipe**) de uma [equipe](../resources/team.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | Channel.Delete.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | Channel.Delete.All |


> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/incomingChannels/{incoming-channel-id}/$ref
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sharedwithchannelteaminfo"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/incomingChannels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/$ref
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sharedwithchannelteaminfo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sharedwithchannelteaminfo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sharedwithchannelteaminfo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sharedwithchannelteaminfo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-sharedwithchannelteaminfo-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-sharedwithchannelteaminfo-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Confira também

- [Remover membro do canal](channel-delete-members.md)
- [Remover membro da equipe](team-delete-members.md)
