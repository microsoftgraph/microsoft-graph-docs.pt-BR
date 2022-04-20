---
title: Tipo de recurso incomingCallOptions
description: Representa uma classe que contém as opções para uma chamada de entrada.
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 700f0139f79415b264544d60386f8b7dba5dc24e
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917801"
---
# <a name="incomingcalloptions-resource-type"></a>Tipo de recurso incomingCallOptions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma classe que contém as opções para uma chamada de entrada.

Herda de [callOptions](calloptions.md).

## <a name="properties"></a>Propriedades

|Propriedade                 |Tipo                      |Descrição                                                                        |
|:---                     |:---                      |:---                                                                               |
|isContentSharingNotificationEnabled   |Boolean                   |O valor que indica se as notificações de compartilhamento de conteúdo devem ser habilitadas para a chamada. Herdado [de callOptions](calloptions.md).    |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.incomingCallOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.incomingCallOptions",
  "isContentSharingNotificationEnabled": "Boolean"
}
```
