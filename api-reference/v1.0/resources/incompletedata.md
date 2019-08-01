---
author: daspek
ms.author: dspektor
title: tipo de recurso incompleteData
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0ac77c5dc4daed9330c4fb71185e9505feee5048
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029236"
---
# <a name="incompletedata-resource-type"></a>tipo de recurso incompleteData

A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.
As propriedades dentro podem fornecer informações sobre o motivo pelo qual os dados estão incompletos.

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo           | Descrição
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | O serviço não tem dados de origem antes do tempo especificado.
| wasThrottled              | Booliano        | Alguns dados não foram gravados devido à atividade excessiva.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->
