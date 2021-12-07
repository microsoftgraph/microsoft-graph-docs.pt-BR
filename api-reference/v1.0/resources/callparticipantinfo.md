---
title: Tipo de recurso callParticipantInfo
description: Representa os detalhes de um participante de chamada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 95b0e796092f2e9f2ddf480b586d9e50eead0380
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322343"
---
# <a name="callparticipantinfo-resource-type"></a>Tipo de recurso callParticipantInfo

Namespace: microsoft.graph

Representa os detalhes de um participante de chamada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|participante|[identitySet](../resources/identityset.md)|Identidade do participante da chamada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callParticipantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callParticipantInfo",
  "participant": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

