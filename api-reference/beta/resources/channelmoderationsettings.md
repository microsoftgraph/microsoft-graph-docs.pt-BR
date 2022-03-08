---
title: Tipo de recurso channelModerationSettings
description: Usado para controlar quem pode iniciar novas postagens e responder a postagens em um canal.
author: anandjo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31538f7b5db717977490fa0b6e37749ef2787edd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337044"
---
# <a name="channelmoderationsettings-resource-type"></a>Tipo de recurso channelModerationSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Microsoft Teams, os proprietários da equipe podem ativar a moderação de um canal para controlar quem pode iniciar novas postagens e responder a postagens nesse canal. Por exemplo, os proprietários podem querer fazer o seguinte:

- Use um canal apenas para anúncios.
- Use um canal para discussões em uma equipe de classe onde somente o professor pode iniciar novas discussões.
- Use um canal para problemas de livesite onde novas postagens podem ser iniciadas por conectores.

Por padrão, a moderação `OFF`é , o que significa que as configurações de canal usuais se aplicam aos proprietários da equipe e aos membros da equipe, com controle adicional para permitir que apenas membros da equipe ou todos, incluindo convidados, iniciem uma nova postagem de canal. Definir moderação de canal permite `ON` que apenas moderadores iniciem novas postagens, com controle adicional para membros da equipe.

Para dar suporte às configurações de moderação de canal por meio de APIs do Microsoft Graph:

- Os membros da equipe devem ser capazes de consultar as configurações de moderação do canal.
- Os proprietários de equipe devem ser capazes de definir as configurações de moderação do canal.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowNewMessageFromBots|Booliano|Indica se os bots têm permissão para postar mensagens.|
|allowNewMessageFromConnectors|Booliano|Indica se os conectores têm permissão para postar mensagens.|
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

- Para modificar as configurações de moderação de um canal, consulte o exemplo 2 no [canal Atualizar](../api/channel-patch.md).
