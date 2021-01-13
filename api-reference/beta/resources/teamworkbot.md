---
title: Tipo de recurso teamworkBot
description: Um bot no ecossistema do Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8c21e7ab3b88c2659bf055e39b931cbc6e9d2f39
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844673"
---
# <a name="teamworkbot-resource-type"></a>Tipo de recurso teamworkBot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um bot no ecossistema do Microsoft Teams.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter bot](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|Leia as propriedades e os relacionamentos de um objeto [teamworkBot.](../resources/teamworkbot.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A id do bot associado ao [teamsAppDefinition específico.](../resources/teamsappdefinition.md) Esse valor geralmente é um GUID.|

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

- Para instalar bots em uma equipe, confira o exemplo 2 em [Listar aplicativos em equipe.](../api/team-list-installedapps.md)
- Para instalar bots em um chat, confira o exemplo 2 em Aplicativos [de lista no chat.](../api/chat-list-installedapps.md)
- Para instalar bots no escopo pessoal de um usuário, confira o exemplo 2 em Aplicativos de [lista instalados para o usuário.](../api/userteamwork-list-installedapps.md)



