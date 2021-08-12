---
title: Tipo de recurso serviceUpdateMessageViewpoint
description: Representa os dados de pontos de exibição do usuário para um serviceUpdateMessage."
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 2d35d04c243469eb72cb0ad85cb269d7de32a4b0642dfb3489963f6f2a294813
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195579"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>Tipo de recurso serviceUpdateMessageViewpoint

Namespace: microsoft.graph

Representa dados de pontos de exibição do usuário para [um serviceUpdateMessage](../resources/serviceupdatemessage.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isArchived|Booliano|Indica se o usuário arquivou a mensagem.|
|isFavorited|Booliano|Indica se o usuário marcou a mensagem como favorita.|
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