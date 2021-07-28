---
title: Tipo de recurso callParticipantInfo
description: Representa os detalhes de um participante de chamada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 59b4837116b8223e41945cd722ae59bef64698c3
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534208"
---
# <a name="callparticipantinfo-resource-type"></a>Tipo de recurso callParticipantInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

