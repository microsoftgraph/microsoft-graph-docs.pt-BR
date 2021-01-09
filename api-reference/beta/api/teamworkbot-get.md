---
title: Obter teamworkBot
description: Leia as propriedades e os relacionamentos de um objeto teamworkBot.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05cb2e8e4d6a41028a9f35b82561b4f5b5d80251
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790584"
---
# <a name="get-teamworkbot"></a>Obter teamworkBot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o bot associado a uma definição [específica](../resources/teamsappdefinition.md) do  [TeamsApp](../resources/teamsapp.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)| AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte aos parâmetros de `$select` [consulta OData](/graph/query-parameter) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [teamworkBot](../resources/teamworkbot.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkBot"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "1f81bb29-bb29-1f81-29bb-811f29bb811f"
}
```
## <a name="see-also"></a>Confira também

- Para instalar bots em uma equipe, confira o exemplo 2 em [Listar aplicativos em equipe.](team-list-installedapps.md)
- Para instalar bots em um chat, confira o exemplo 2 em Aplicativos [de lista no chat.](chat-list-installedapps.md)
- Para instalar bots no escopo pessoal de um usuário, confira o exemplo 2 em Aplicativos de [lista instalados para o usuário.](userteamwork-list-installedapps.md)


