---
title: Tipo de recurso serviceHealthIssuePost
description: Representa uma postagem histórica em um problema de saúde do serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c005beb7b27956cad6f42c7251bb15be7024415c5096d8f012a88049534b6cad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243006"
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

