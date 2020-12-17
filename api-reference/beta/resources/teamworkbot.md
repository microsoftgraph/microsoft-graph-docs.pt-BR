---
title: tipo de recurso teamworkBot
description: Um bot no ecossistema do Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 383c646fdb30d082daa73e37fd227238db195b6b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706255"
---
# <a name="teamworkbot-resource-type"></a>tipo de recurso teamworkBot

Namespace: microsoft.graph

Representa um bot no ecossistema do Microsoft Teams.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter bot](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|Leia as propriedades e os relacionamentos de um objeto [teamworkBot](../resources/teamworkbot.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do bot associada ao [teamsAppDefinition](../resources/teamsappdefinition.md)específico. Esse valor geralmente é um GUID.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a>Confira também

- Para obter bots instalados em uma equipe, confira o exemplo 2 em [list apps in Team](../api/team-list-installedapps.md).
- Para obter bots instalados em um chat, confira o exemplo 2 em [listar aplicativos no chat](../api/chat-list-installedapps.md).
- Para obter bots instalados no escopo pessoal de um usuário, confira o exemplo 2 em [listar aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md).



