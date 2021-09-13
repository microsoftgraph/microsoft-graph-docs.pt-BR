---
title: Tipo de recurso educationExcelResource
description: Uma subclasse de educationResource. Esse tipo de recurso representa um Excel documento.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0e91d927e493a578a5a067e5a1caa1795a066940
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59099025"
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


