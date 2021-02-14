---
author: daspek
title: Tipo de recurso incompleteData
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 20dda8e9d1cd321a465c7a257cb5cb7bed845351
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239930"
---
# <a name="incompletedata-resource-type"></a>Tipo de recurso incompleteData

Namespace: microsoft.graph

A **faceta incompleteData** indica que um recurso foi gerado com dados incompletos.
As propriedades dentro podem fornecer informações sobre por que os dados estão incompletos.

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo           | Descrição
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | O serviço não tem dados de origem antes da hora especificada.
| wasThrottled              | Booliano        | Alguns dados não foram registrados devido a atividade excessiva.

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

