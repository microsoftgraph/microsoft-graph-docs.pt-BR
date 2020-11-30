---
title: tipo de recurso teamworkActivityTopic
description: Representa o tópico de uma notificação de feed de atividade.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a4425053cf41ebfbad139c6d0ea5fc246f0b1391
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377490"
---
# <a name="teamworkactivitytopic-resource-type"></a>tipo de recurso teamworkActivityTopic

Namespace: microsoft.graph

Representa o tópico de uma notificação de feed de atividade.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|source|teamworkActivityTopicSource|Tipo de fonte. Os valores possíveis são: `entityUrl` e `text`. Para obter suporte para URLs do Microsoft Graph, use `entityUrl` . Para texto personalizado, use `text` .|
|value|Cadeia de caracteres|O valor do tópico. Se o valor da propriedade **Source** for `entityUrl` , ele deve ser uma URL do Microsoft Graph. Se o vaule for `text` , ele deverá ser um valor de texto sem formatação.|
|webUrl|String|O link que o usuário clica quando seleciona a notificação. Opcional quando **Source** é `entityUrl` ; Required quando **Source** é `text` .|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivityTopic"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.teamworkActivityTopic",
  "source": "String",
  "value": "String",
  "webUrl": "String"
}
```

