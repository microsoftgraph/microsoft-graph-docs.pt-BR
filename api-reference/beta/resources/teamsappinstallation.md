---
title: Tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou um escopo pessoal do usuário. '
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 85bac3f22ad609b2914a4a1d36b0d09f2e3d85e2
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943672"
---
# <a name="teamsappinstallation-resource-type"></a>Tipo de recurso teamsAppInstallation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um [teamsApp](teamsapp.md) instalado em uma [equipe,](team.md) [um chat](chat.md)ou o escopo pessoal de um [usuário.](user.md) Todos os bots que fazem parte do aplicativo se tornarão parte de qualquer equipe, chat ou escopo pessoal do usuário ao que o aplicativo é adicionado.

> [!NOTE]
> O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos em equipe](../api/team-list-installedapps.md) | Coleção [teamsAppInstallation](teamsappinstallation.md) | Liste os aplicativos instalados em uma equipe.|
|[Instalar o aplicativo na equipe do](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obtenha o aplicativo especificado instalado em uma equipe.|
|[Adicionar aplicativo à equipe](../api/team-post-installedapps.md) |Nenhuma | Adicione (instale) um aplicativo a uma equipe.|
|[Atualizar o aplicativo instalado para a equipe](../api/team-teamsappinstallation-upgrade.md) | Nenhuma | Atualize o aplicativo instalado em uma equipe para a versão mais recente.|
|[Remover aplicativo da equipe](../api/team-delete-installedapps.md) | Nenhuma | Remova (desinstale) um aplicativo de uma equipe.|
|[Lista de aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md) | Coleção[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Listar aplicativos instalados no escopo pessoal de um usuário.|
|[Obter aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Instale o aplicativo especificado no escopo pessoal de um usuário. |
|[Adicionar o aplicativo para o usuário](../api/userteamwork-post-installedapps.md) | | Adicionar (instalar) um aplicativo no escopo pessoal de um usuário.|
|[Atualizar o aplicativo instalado para o usuário](../api/userteamwork-teamsappinstallation-upgrade.md) | Nenhum | Atualize o aplicativo instalado no escopo pessoal de um usuário para a versão mais recente.|
|[Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remova (desinstale) um aplicativo no escopo pessoal de um usuário.|
|[Listar aplicativos no chat](../api/chat-list-installedapps.md) |Coleção [teamsAppInstallation](teamsappinstallation.md) | Listar aplicativos instalados em um chat.|
|[Obter aplicativo instalado no chat](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Instale o aplicativo especificado em um chat.|
|[Adicionar aplicativo no chat](../api/chat-post-installedapps.md) | | Adicionar (instalar) um aplicativo a um chat.|
|[Atualizar aplicativo no chat](../api/chat-teamsappinstallation-upgrade.md) | Nenhum | Atualize o aplicativo instalado em um chat para a versão mais recente.|
|[Remover aplicativo do chat](../api/chat-delete-installedapps.md) | Nenhum | Remova (desinstalar) o aplicativo de um chat.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não a ID do aplicativo da equipe). |

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


