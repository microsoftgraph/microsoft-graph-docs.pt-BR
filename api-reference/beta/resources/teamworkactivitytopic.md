---
title: Tipo de recurso teamworkActivityTopic
description: Representa o tópico de uma notificação de feed de atividade.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fe34a16382d3a2e806fd0c95fe9d09d55c3e2dbea4f3cea1e7d861f05f9af1b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185464"
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

