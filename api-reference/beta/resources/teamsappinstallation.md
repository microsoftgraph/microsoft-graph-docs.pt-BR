---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou o escopo pessoal de um usuário. '
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 66cf31f21a105934181aee5e506cc2215f9ce7a9
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663902"
---
# <a name="teamsappinstallation-resource-type"></a>tipo de recurso teamsAppInstallation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md), um [chat](chat.md)ou o escopo pessoal de um [usuário](user.md). Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe, chat ou escopo pessoal do usuário ao qual o aplicativo é adicionado.

> [!NOTE]
> O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos instalados no Team](../api/team-list-installedapps.md) | Coleção [teamsAppInstallation](teamsappinstallation.md) | Listar aplicativos instalados em uma equipe.|
|[Obter o aplicativo instalado no Team](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obtenha o aplicativo especificado instalado em uma equipe.|
|[Adicionar aplicativo à equipe](../api/team-post-installedapps.md) |Nenhum | Adicionar (instalar) um aplicativo a uma equipe.|
|[Atualizar aplicativo instalado no Team](../api/team-teamsappinstallation-upgrade.md) | Nenhum | Atualize o aplicativo instalado em uma equipe para a versão mais recente.|
|[Remover aplicativo da equipe](../api/team-delete-installedapps.md) | Nenhum | Remova (desinstale) um aplicativo de uma equipe.|
|[Lista de aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md) | Coleção[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Listar aplicativos instalados no escopo pessoal de um usuário.|
|[Obter o aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Obtenha o aplicativo especificado instalado no escopo pessoal de um usuário. |
|[Adicionar o aplicativo para o usuário](../api/userteamwork-post-installedapps.md) | | Adicionar (instalar) um aplicativo no escopo pessoal de um usuário.|
|[Atualizar o aplicativo instalado para o usuário](../api/userteamwork-teamsappinstallation-upgrade.md) | Nenhum | Atualize o aplicativo instalado no escopo pessoal de um usuário para a versão mais recente.|
|[Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remova (desinstale) um aplicativo no escopo pessoal de um usuário.|
|[Listar aplicativos no chat](../api/chat-list-installedapps.md) |Coleção [teamsAppInstallation](teamsappinstallation.md) | Listar aplicativos instalados em um chat.|
|[Obter o aplicativo instalado no chat](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obtenha o aplicativo especificado instalado em um chat.|
|[Adicionar aplicativo ao chat](../api/chat-post-installedapps.md) | | Adicionar (instalar) um aplicativo a um chat.|
|[Atualizar aplicativo no chat](../api/chat-teamsappinstallation-upgrade.md) | Nenhum | Atualize o aplicativo instalado em um chat para a versão mais recente.|
|[Remover aplicativo de chat](../api/chat-delete-installedapps.md) | Nenhum | Remova (desinstale) o aplicativo de um chat.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não a ID de AP da equipe). |

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
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


