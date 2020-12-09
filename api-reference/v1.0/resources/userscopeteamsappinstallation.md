---
title: tipo de recurso userScopeTeamsAppInstallation
description: Representa um teamsApp instalado no escopo pessoal de um usuário.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 30df2c14f8723dedd25fb7c4e5b2a00481338dc3
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606857"
---
# <a name="userscopeteamsappinstallation-resource-type"></a>tipo de recurso userScopeTeamsAppInstallation

Namespace: Microsoft Graph

Representa um [teamsApp](teamsapp.md) instalado no escopo pessoal de um [usuário](user.md). Qualquer bots que faça parte do aplicativo se tornará parte do escopo pessoal de um usuário ao qual o aplicativo é adicionado.
Este tipo herda de [teamsAppInstallation](teamsappinstallation.md).

> [!NOTE]
> O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md)| coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Listar aplicativos instalados no escopo pessoal de um usuário. |
|[Obtém o aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Lista o aplicativo especificado instalado no escopo pessoal de um usuário. |
|[Adicionar aplicativo para usuário](../api/userteamwork-post-installedapps.md) | Nenhum | Adicionar (instalar) um aplicativo no escopo pessoal de um usuário. |
|[Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remova (desinstale) um aplicativo no escopo pessoal de um usuário. |
|[Atualizar o aplicativo instalado para o usuário](../api/userteamwork-teamsappinstallation-upgrade.md) | Nenhum | Atualize para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.|
|[Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md) | Listar chats de um-on-one entre um usuário e o aplicativo. |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | cadeia de caracteres   | Uma ID exclusiva (não a ID do aplicativo Teams). |

## <a name="relationships"></a>Relações

| Relação   | Tipo    | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| O aplicativo que está instalado. |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| Os detalhes desta versão do aplicativo. |
|chat |[chat](chat.md) | O chat entre o usuário e o aplicativo do teams. | 

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

