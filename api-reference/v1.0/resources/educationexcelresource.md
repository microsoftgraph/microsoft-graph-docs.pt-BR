---
title: Tipo de recurso educationExcelResource
description: Uma subclasse de educationResource. Esse tipo de recurso representa um Excel documento.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9345bb39f16066b4c5eee688d781e99563147ef2
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912112"
---
# <a name="educationexcelresource-resource-type"></a>Tipo de recurso educationExcelResource

Namespace: microsoft.graph

Uma subclasse [de educationResource](educationresource.md). Esse tipo de recurso representa um Excel documento.  
 
>**Observação:** O Excel arquivo deve estar na pasta de recursos associada ao objeto de atribuição ou envio ao qual esse recurso pertence.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|String|Ponteiro para o objeto Excel arquivo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


