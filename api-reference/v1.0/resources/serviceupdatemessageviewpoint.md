---
title: Tipo de recurso serviceUpdateMessageViewpoint
description: Representa os dados de pontos de exibição do usuário para um serviceUpdateMessage."
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 57d5bf64069d0799514eafc78fbfb5d221ccf82b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58250894"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>Tipo de recurso serviceUpdateMessageViewpoint

Namespace: microsoft.graph

Representa dados de pontos de exibição do usuário para [um serviceUpdateMessage](../resources/serviceupdatemessage.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isArchived|Booliano|Indica se o usuário arquivou a mensagem.|
|isFavorited|Boolean|Indica se o usuário marcou a mensagem como favorita.|
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