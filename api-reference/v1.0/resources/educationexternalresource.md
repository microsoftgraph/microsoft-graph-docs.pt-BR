---
title: Tipo de recurso educationExternalResource
description: Uma subclasse de educationResource. Esse é o serviço padrão de atribuições de tipo de recurso usado para mapear todos os recursos que não expomos ao gráfico. Isso permite que todos os chamadores SDK funcionem perfeitamente.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3bfefee10d387a34c783c3f8afec7ee00480a506
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220785"
---
# <a name="educationexternalresource-resource-type"></a>Tipo de recurso educationExternalResource

Namespace: microsoft.graph

Representa um tipo genérico para mapear recursos não expostos no Microsoft Graph.

Herda de [educationResource](educationresource.md).

Esse tipo complexo permite que todos os chamadores SDK funcionem perfeitamente.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|webUrl|String|Local do recurso. Obrigatório|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationExternalResource"
}-->

```json
{
  "webUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-09-21 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExternalResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
