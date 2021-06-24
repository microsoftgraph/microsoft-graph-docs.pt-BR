---
title: Tipo de recurso serviceHealthIssuePost
description: Representa uma postagem histórica em um problema de saúde do serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 910236d2059f951169bea314a0b38ae2516b1918
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107768"
---
# <a name="servicehealthissuepost-resource-type"></a>Tipo de recurso serviceHealthIssuePost

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma postagem histórica em um [problema de saúde do serviço.](../resources/servicehealthissue.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|O horário publicado da postagem.|
|description|[itemBody](../resources/itembody.md)|O conteúdo da postagem de problema do serviço.|
|postType|postType|O tipo de postagem da postagem histórica do problema do serviço. Os valores possíveis são: `regular`, `quick`, `strategic`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceHealthIssuePost"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssuePost",
  "createdDateTime": "String (timestamp)",
  "postType": "String",
  "description": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

