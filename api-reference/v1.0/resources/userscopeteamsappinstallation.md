---
title: tipo de recurso userScopeTeamsAppInstallation
description: Representa um teamsApp instalado no escopo pessoal de um usuário.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8e485b2a4c5bf056202e94adaaa754c378a06936
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564009"
---
# <a name="userscopeteamsappinstallation-resource-type"></a>tipo de recurso userScopeTeamsAppInstallation

Namespace: microsoft.graph

Representa um [teamsApp](teamsapp.md) instalado no escopo pessoal de um [usuário](user.md). Qualquer bots que faça parte do aplicativo se tornará parte do escopo pessoal de um usuário ao qual o aplicativo é adicionado.
Este tipo herda de [teamsAppInstallation](teamsappinstallation.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md)| coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Listar aplicativos instalados no escopo pessoal de um usuário. |
|[Obtém o aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Lista o aplicativo especificado instalado no escopo pessoal de um usuário. |
|[Adicionar aplicativo para usuário](../api/userteamwork-add-installedapps.md) | Nenhum | Adiciona (instala) um aplicativo no escopo pessoal de um usuário. |
|[Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remove (desinstala) um aplicativo no escopo pessoal de um usuário. |
|[Atualizar o aplicativo instalado para o usuário](../api/userteamwork-upgrade-installedapps.md) | Nenhum | Atualiza para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.|
|[Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md) | Lista o chat de um em um entre o usuário e o aplicativo. |

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

