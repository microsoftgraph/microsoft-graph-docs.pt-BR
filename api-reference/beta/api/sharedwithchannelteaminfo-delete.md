---
title: Excluir sharedWithChannelTeamInfo
description: Exclua uma equipe de um canal compartilhado.
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 899bc9a9b60f1d7bb8bba8fec89e2bd311be7bae
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060567"
---
# <a name="delete-sharedwithchannelteaminfo"></a>Excluir sharedWithChannelTeamInfo
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descompartilhar um [canal](../resources/channel.md) com uma [equipe](../resources/team.md) excluindo o recurso [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) correspondente. Esta operação é permitida somente para canais com valor **membershipType** de `shared`.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | ChannelMember.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | ChannelMember.ReadWrite.All |


> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/channels/{channel-id}/sharedWithTeams/{shared-with-channel-team-info-id}
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

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "delete_sharedwithchannelteaminfo"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/sharedWithTeams/ece6f0a1-5g39-498b-be79-edf6c8fc4d82
```


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
