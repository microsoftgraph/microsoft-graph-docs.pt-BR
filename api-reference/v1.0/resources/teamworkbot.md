---
title: Tipo de recurso do teamworkBot
description: Um bot no ecossistema do Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99bdde9a4ff26945dd5aa040f2741fdf50c1273b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476402"
---
# <a name="teamworkbot-resource-type"></a>Tipo de recurso do teamworkBot

Namespace: microsoft.graph

Representa um bot no ecossistema do Microsoft Teams.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter bot](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|Leia as propriedades e as relações de um objeto [teamworkBot.](../resources/teamworkbot.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do bot associado ao [teamsAppDefinition específico.](../resources/teamsappdefinition.md) Esse valor geralmente é um GUID.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
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

- Para instalar bots em uma equipe, consulte o exemplo 2 em [Listar aplicativos em equipe](../api/team-list-installedapps.md). <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md). -->
- Para instalar bots no escopo pessoal de um usuário, consulte o exemplo 2 em Aplicativos de [lista instalados para usuário](../api/userteamwork-list-installedapps.md).



