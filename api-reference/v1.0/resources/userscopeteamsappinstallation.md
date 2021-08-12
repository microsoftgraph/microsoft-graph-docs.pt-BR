---
title: Tipo de recurso userScopeTeamsAppInstallation
description: Representa um teamsApp instalado no escopo pessoal de um usuário.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 46532e7808e30359c82448287fcdbcf0dd87a75421fdff7012e77792f02d0212
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54211820"
---
# <a name="userscopeteamsappinstallation-resource-type"></a>Tipo de recurso userScopeTeamsAppInstallation

Namespace: microsoft.graph

Representa um [teamsApp](teamsapp.md) instalado no escopo pessoal de um [usuário](user.md). Todos os bots que fazem parte do aplicativo se tornarão parte do escopo pessoal de um usuário ao que o aplicativo é adicionado.
Esse tipo herda de [teamsAppInstallation](teamsappinstallation.md).

> [!NOTE]
> O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Lista de aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md)| Coleção[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Listar aplicativos instalados no escopo pessoal de um usuário. |
|[Obtém o aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Listar o aplicativo especificado instalado no escopo pessoal de um usuário. |
|[Adicionar o aplicativo para o usuário](../api/userteamwork-post-installedapps.md) | Nenhum | Adicionar (instalar) um aplicativo no escopo pessoal de um usuário. |
|[Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remover (desinstalar) um aplicativo no escopo pessoal de um usuário. |
|[Atualizar o aplicativo instalado para o usuário](../api/userteamwork-teamsappinstallation-upgrade.md) | Nenhum | Atualize para a versão mais recente do aplicativo instalada no escopo pessoal de um usuário.|
|[Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md) | Listar chats um-a-um entre um usuário e o aplicativo. |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não Teams ID do aplicativo). |

## <a name="relationships"></a>Relações

| Relação   | Tipo    | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| O aplicativo instalado. |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| Os detalhes dessa versão do aplicativo. |
|chat |[chat](chat.md) | O chat entre o usuário e o Teams app. | 

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userScopeTeamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a>Confira também

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userScopeTeamsAppInstallation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

