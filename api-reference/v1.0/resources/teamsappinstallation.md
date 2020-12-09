---
title: tipo de recurso teamsAppInstallation
description: Representa um teamsApp instalado em uma equipe ou o escopo pessoal de um usuário.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c872d41ebc09978d9dc54ac01d82cb33258541d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607032"
---
# <a name="teamsappinstallation-resource-type"></a>tipo de recurso teamsAppInstallation

Namespace: Microsoft Graph

Representa um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md) ou o escopo pessoal de um [usuário](user.md). Qualquer bots que faça parte do aplicativo se tornará parte de qualquer escopo pessoal do usuário ou da equipe ao qual o aplicativo é adicionado.

> [!NOTE]
> O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos instalados no Team](../api/team-list-installedapps.md) | Coleção [teamsAppInstallation](teamsappinstallation.md) | Listar aplicativos instalados em uma equipe.|
|[Obter o aplicativo instalado em uma equipe](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obtenha o aplicativo especificado instalado em uma equipe.|
|[Adicionar aplicativo à equipe](../api/team-post-installedapps.md) |Nenhum | Adicionar (instalar) um aplicativo a uma equipe.|
|[Remover aplicativo da equipe](../api/team-delete-installedapps.md) | Nenhum | Remova (desinstale) um aplicativo de uma equipe.|
|[Atualizar aplicativo instalado no Team](../api/team-teamsappinstallation-upgrade.md) | Nenhum | Atualize o aplicativo instalado em uma equipe para a versão mais recente.|
|[Listar aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md) | coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Listar aplicativos instalados no escopo pessoal de um usuário.|
|[Obter o aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Obtenha o aplicativo especificado instalado no escopo pessoal de um usuário. |
|[Adicionar aplicativo para usuário](../api/userteamwork-post-installedapps.md) | | Adicionar (instalar) um aplicativo no escopo pessoal de um usuário.|
|[Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remova (desinstale) um aplicativo no escopo pessoal de um usuário.|
|[Atualizar o aplicativo instalado para o usuário](../api/userteamwork-teamsappinstallation-upgrade.md) | Nenhum | Atualize o aplicativo instalado no escopo pessoal de um usuário para a versão mais recente.|


## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | cadeia de caracteres   | Uma ID exclusiva (não a ID do aplicativo Teams). |

## <a name="relationships"></a>Relações

| Relação   | Tipo    | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| O aplicativo que está instalado. |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| Os detalhes desta versão do aplicativo. |


## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
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
- [userScopeTeamsAppInstallation](../resources/userscopeteamsappinstallation.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

