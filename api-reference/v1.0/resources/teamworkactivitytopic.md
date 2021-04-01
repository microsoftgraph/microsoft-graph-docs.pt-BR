---
title: Tipo de recurso teamworkActivityTopic
description: Representa o tópico de uma notificação de feed de atividade.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abf2372aca7d58061f609c97521795f328af89f6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473987"
---
# <a name="teamworkactivitytopic-resource-type"></a>Tipo de recurso teamworkActivityTopic

Namespace: microsoft.graph

Representa o tópico de uma notificação de feed de atividade.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|source|teamworkActivityTopicSource|Tipo de fonte. Os valores possíveis são: `entityUrl` e `text`. Para URLs do Microsoft Graph com suporte, use `entityUrl` . Para texto personalizado, use `text` .|
|value|Cadeia de caracteres|O valor do tópico. Se o valor da **propriedade de origem** for `entityUrl` , deve ser uma URL do Microsoft Graph. Se o vaule for `text` , este deve ser um valor de texto simples.|
|webUrl|String|O link que o usuário clica ao selecionar a notificação. Opcional quando **a origem** `entityUrl` for ; obrigatório quando a **origem** for `text` .|

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

