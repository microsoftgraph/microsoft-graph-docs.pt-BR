---
title: tipo de recurso channelModerationSettings
description: Usado para controlar quem pode iniciar novas postagens e responder a postagens em um canal.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2de1c16ed998a0b793d14c6a4d791613e0bef62
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706213"
---
# <a name="channelmoderationsettings-resource-type"></a>tipo de recurso channelModerationSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Microsoft Teams, os proprietários de equipe podem ativar a moderação de um canal para controlar quem pode iniciar novas postagens e responder a postagens nesse canal. Por exemplo, os proprietários podem querer fazer o seguinte:

- Usar um canal somente para comunicados.
- Use um canal para discussões em uma equipe de aula onde apenas o professor pode iniciar novas discussões.
- Use um canal para problemas de Livesite onde novas postagens podem ser iniciadas por conectores.

Por padrão, a moderação é `OFF` , o que significa que as configurações de canal usuais se aplicam aos proprietários da equipe e aos membros da equipe, com controle adicional para permitir que somente membros da equipe ou todos, incluindo convidados, iniciem uma nova postagem de canal. Configurar a moderação do canal para `ON` permitir que apenas moderadores iniciem novas postagens, com controle adicional para membros da equipe.

Para dar suporte às configurações de moderação de canal através das APIs do Microsoft Graph:

- Os membros da equipe devem ser capazes de consultar as configurações de moderação do canal.
- Os proprietários de equipe devem ser capazes de definir as configurações de moderação do canal.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowNewMessageFromBots|Boolean|Indica se os bots podem postar mensagens.|
|allowNewMessageFromConnectors|Boolean|Indica se os conectores têm permissão para postar mensagens.|
|replyRestriction|replyRestriction|Indica quem tem permissão para responder ao canal Teams. Os valores possíveis são: `everyone`, `authorAndModerators`, `unknownFutureValue`.|
|userNewMessageRestriction|userNewMessageRestriction|Indica quem tem permissão para postar mensagens no canal do teams. Os valores possíveis são: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelModerationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelModerationSettings",
  "userNewMessageRestriction": "String",
  "replyRestriction": "String",
  "allowNewMessageFromBots": "Boolean",
  "allowNewMessageFromConnectors": "Boolean"
}
```
