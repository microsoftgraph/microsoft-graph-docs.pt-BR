---
title: Tipo de recurso serviceUpdateMessageViewpoint
description: Representa os dados de pontos de exibição do usuário para um serviceUpdateMessage."
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c84a07691c2507a9ff74102ac6f4b1675cb382e7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109062"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>Tipo de recurso serviceUpdateMessageViewpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados de pontos de exibição do usuário para [um serviceUpdateMessage](../resources/serviceupdatemessage.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isArchived|Booliano|Indica se o usuário arquivou a mensagem.|
|isFavorited|Booleano|Indica se o usuário marcou a mensagem como favorita.|
|isRead|Boolean|Indica se o usuário leu a mensagem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessageViewpoint",
  "isRead": "Boolean",
  "isArchived": "Boolean",
  "isFavorited": "Boolean"
}
```