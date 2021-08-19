---
title: Tipo de recurso serviceHealthIssuePost
description: Representa uma postagem histórica em um problema de saúde do serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: a53f09c6fc32de1c65e52e2554aa89b634f2b0e3
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266895"
---
# <a name="servicehealthissuepost-resource-type"></a>Tipo de recurso serviceHealthIssuePost

Namespace: microsoft.graph

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

