---
title: Tipo de recurso teamworkActivityTopic
description: Representa o tópico de uma notificação de feed de atividade.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0438234e1e771fc822cf2f5d5742ffa14cf72e36
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123899"
---
# <a name="teamworkactivitytopic-resource-type"></a>Tipo de recurso teamworkActivityTopic

Namespace: microsoft.graph

Representa o tópico de uma notificação de feed de atividade.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|source|teamworkActivityTopicSource|Tipo de fonte. Os valores possíveis são: `entityUrl` e `text`. Para URLs Graph Microsoft com suporte, use `entityUrl` . Para texto personalizado, use `text` .|
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

