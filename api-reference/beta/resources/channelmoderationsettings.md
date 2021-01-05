---
title: tipo de recurso channelModerationSettings
description: Usado para controlar quem pode iniciar novas postagens e responder a postagens em um canal.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: db3618528aef9b5ec562bbb80a6298f9e5f05b34
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754135"
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
|allowNewMessageFromBots|Booliano|Indica se os bots podem postar mensagens.|
|allowNewMessageFromConnectors|Booliano|Indica se os conectores têm permissão para postar mensagens.|
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

## <a name="see-also"></a>Confira também

- Para modificar as configurações de moderação de um canal, confira o exemplo 2 em [canal de atualização](../api/channel-patch.md).