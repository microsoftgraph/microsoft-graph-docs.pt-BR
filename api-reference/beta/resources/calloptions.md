---
title: Tipo de recurso callOptions
description: Uma classe base abstrata que contém os recursos opcionais para uma chamada.
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 53d845d7667f04f5b028fdde01b2658e578a7a25
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917819"
---
# <a name="calloptions-resource-type"></a>Tipo de recurso callOptions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma classe base abstrata que contém os recursos opcionais para uma chamada.

## <a name="properties"></a>Propriedades

|Propriedade                 |Tipo                      |Descrição                                                                        |
|:---                     |:---                      |:---                                                                               |
|isContentSharingNotificationEnabled   |Boolean                   |Indica se as notificações de compartilhamento de conteúdo devem ser habilitadas para a chamada.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callOptions",
  "isContentSharingNotificationEnabled": "Boolean"
}
```
