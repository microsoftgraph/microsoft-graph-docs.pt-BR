---
title: Tipo de recurso educationExcelResource
description: Uma subclasse de educationResource. Esse tipo de recurso representa um Excel documento.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 39f74b488351ddca954db696f9c8ec3bfe5ff97b86d294b5dd2162e199d6c849
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252022"
---
# <a name="educationexcelresource-resource-type"></a>Tipo de recurso educationExcelResource

Namespace: microsoft.graph

Uma subclasse [de educationResource](educationresource.md). Esse tipo de recurso representa um Excel documento.  
 
>**Observação:** O Excel arquivo deve estar na pasta de recursos associada ao objeto de atribuição ou envio ao qual esse recurso pertence.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|Cadeia de caracteres|Ponteiro para o objeto Excel arquivo.|

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


