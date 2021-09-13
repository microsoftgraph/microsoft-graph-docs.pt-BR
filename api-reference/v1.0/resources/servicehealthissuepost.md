---
title: Tipo de recurso serviceHealthIssuePost
description: Representa uma postagem histórica em um problema de saúde do serviço.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 3216f0a4510b6dd66a0ce5c7a96834dbf289b378
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126671"
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

