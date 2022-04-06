---
title: Listar associatedTeamInfo
description: Obtenha a lista de equipes Microsoft Teams a que um usuário está associado.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16842866ca4c2b03268e80eb838bbf953844c605
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685261"
---
# <a name="list-associatedteaminfo"></a>Listar associatedTeamInfo
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a lista de [equipes](../resources/associatedteaminfo.md) Microsoft Teams a [que um](../resources/user.md) usuário está associado.
Atualmente, um [usuário pode](../resources/user.md) ser associado a uma [equipe](../resources/team.md) de duas maneiras diferentes:
* Um [usuário](../resources/user.md) pode ser um membro direto de uma [equipe](../resources/team.md).
* Um [usuário](../resources/user.md) pode ser membro de um canal [compartilhado](../resources/channel.md) hospedado dentro de uma [equipe](../resources/team.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All|

> **Observação:** atualmente, com as permissões delegadas pelo usuário, essa operação só funcionará para o usuário `me`. Com as permissões de aplicativo, ela funciona para todos os usuários especificando a ID de usuário específica (a alias`me` não é suportada com as permissões de aplicativo).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{user-id}/teamwork/associatedTeams
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
No momento, esse método não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de [objetos AssociatedTeamInfo](../resources/associatedteaminfo.md) no corpo da resposta.

> **Observação**: essa API também retorna a equipe de host do canal compartilhado do qual o usuário é membro direto.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "list_associatedteaminfo"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/teamwork/associatedTeams
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.associatedTeamInfo",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.associatedTeamInfo",
      "id": "b695c5a5-c5a5-b695-a5c5-95b6a5c595b6",
      "tenantId": "172b0cce-e65d-7hd4-9a49-91d9f2e8493a",
      "displayName": "Contoso Team"
    },
    {
      "@odata.type": "#microsoft.graph.associatedTeamInfo",
      "id": "b695c5a5-8934-b695-a5c5-95b6a5c595b6",
      "tenantId": "172b0cce-8961-7hd4-9a49-91d9f2e8493a",
      "displayName": "Fabrikam Team"
    }
  ]
}
```


## <a name="see-also"></a>Confira também

- [Listar joinedTeams](../api/user-list-joinedteams.md)
- [Listar todas as equipes em uma organização](../api/teams-list.md)
- [Obter equipe](../api/team-get.md)

