---
title: Tipo de recurso channelModerationSettings
description: Usado para controlar quem pode iniciar novas postagens e responder a postagens em um canal.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b67d55eb57d1a4b554b027270f700cbd590d4416
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796581"
---
# <a name="channelmoderationsettings-resource-type"></a>Tipo de recurso channelModerationSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Microsoft Teams, os proprietários de equipe podem ativar a moderação para um canal para controlar quem pode iniciar novas postagens e responder a postagens nesse canal. Por exemplo, os proprietários podem querer fazer o seguinte:

- Use um canal somente para comunicados.
- Use um canal para discussões em uma equipe de classe onde somente o professor pode iniciar novas discussões.
- Use um canal para problemas em que novas postagens podem ser iniciadas por conectores.

Por padrão, a moderação é, o que significa que as configurações usuais de canal se aplicam aos proprietários da equipe e membros da equipe, com controle adicional para permitir que apenas membros da equipe ou todos, incluindo convidados, iniciem uma nova postagem de `OFF` canal. Configurar a moderação do canal `ON` para permitir que apenas moderadores iniciem novas postagens, com controle adicional para membros da equipe.

Para dar suporte às configurações de moderação de canal por meio das APIs do Microsoft Graph:

- Os membros da equipe devem ser capazes de consultar as configurações de moderação do canal.
- Os proprietários de equipe devem ser capazes de definir configurações de moderação de canal.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowNewMessageFromBots|Boolean|Indica se os bots têm permissão para postar mensagens.|
|allowNewMessageFromConnectors|Boolean|Indica se os conectores têm permissão para postar mensagens.|
|replyRestriction|replyRestriction|Indica quem tem permissão para responder ao canal de equipes. Os valores possíveis são: `everyone`, `authorAndModerators`, `unknownFutureValue`.|
|userNewMessageRestriction|userNewMessageRestriction|Indica quem tem permissão para postar mensagens no canal de equipes. Os valores possíveis são: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.|

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

- Para modificar as configurações de moderação de um canal, consulte o exemplo 2 no [canal de atualização.](../api/channel-patch.md)
