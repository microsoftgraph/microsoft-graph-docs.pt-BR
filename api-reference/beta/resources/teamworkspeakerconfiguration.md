---
title: Tipo de recurso teamworkSpeakerConfiguration
description: Representa os detalhes sobre a configuração do alto-falante para um Salas do Microsoft Teams dispositivo.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88c15b97ea1b2d3984f8e3c3c4a41873fc228ad0
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262250"
---
# <a name="teamworkspeakerconfiguration-resource-type"></a>Tipo de recurso teamworkSpeakerConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a configuração do alto-falante para um Salas do Microsoft Teams [dispositivo](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isCommunicationSpeakerOptional|Booliano|`True` se o alto-falante de comunicação for opcional. Usado para calcular o estado de saúde se o alto-falante de comunicação não for opcional.|
|isSpeakerOptional|Booliano|`True` se o alto-falante configurado for opcional. Usado para calcular o estado de saúde se o alto-falante não for opcional.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|defaultCommunicationSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|O alto-falante de comunicação padrão usado para reuniões de conferência.|
|defaultSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|O alto-falante padrão usado para todos os sons de mídia e notificação.|
|falantes|[coleção teamworkPeripheral](../resources/teamworkperipheral.md)|A lista de alto-falantes conectados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSpeakerConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSpeakerConfiguration",
  "isCommunicationSpeakerOptional": "Boolean",
  "isSpeakerOptional": "Boolean"
}
```

