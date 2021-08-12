---
title: Tipo de recurso educationWordResource
description: Uma subclasse de educationResource.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00ce0d3a31c62bc38c6a5f9893c69b51a58c3a32741e993691e234a753278385
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192527"
---
# <a name="educationwordresource-resource-type"></a>Tipo de recurso educationWordResource

Namespace: microsoft.graph

Uma subclasse [de educationResource](educationresource.md). 

Este é um recurso de documento do Word. O arquivo word deve ser carregado no **diretório fileResource** associado à atribuição ou ao envio.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|Cadeia de caracteres|Local do arquivo no disco.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


