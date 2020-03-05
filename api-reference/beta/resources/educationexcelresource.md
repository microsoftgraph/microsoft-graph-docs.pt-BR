---
title: tipo de recurso educationExcelResource
description: 'Uma subclasse de educationResource. Esse tipo de recurso representa um documento do Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b533d5072ab9a4e880b14b64e96f4791db399e09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502162"
---
# <a name="educationexcelresource-resource-type"></a>tipo de recurso educationExcelResource

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma subclasse de [educationResource](educationresource.md). Esse tipo de recurso representa um documento do Excel.  
 
>**Observação:** O arquivo do Excel deve estar na pasta de recursos associada à atribuição ou ao objeto de envio ao qual este recurso pertence.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|String|Ponteiro para o objeto de arquivo do Excel.|

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
