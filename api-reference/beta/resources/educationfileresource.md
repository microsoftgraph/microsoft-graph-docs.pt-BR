---
title: tipo de recurso educationFileResource
description: Uma subclasse de educationResource que representa um objeto File associado à atribuição ou ao envio.  Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem tratamento especial no sistema. O recurso de arquivo deve ser armazenado no **resourceFolder** que está associado à atribuição ou ao envio ao qual este recurso está anexado.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 678591d4c9662f1ab3fc68f7d35a0ec525c6e74f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972737"
---
# <a name="educationfileresource-resource-type"></a>tipo de recurso educationFileResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma subclasse de [educationResource](educationresource.md) que representa um objeto File associado à atribuição ou ao envio.  Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem tratamento especial no sistema. O recurso de arquivo deve ser armazenado no **resourceFolder** que está associado à atribuição ou ao envio ao qual este recurso está anexado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|String|Local no disco do recurso de arquivo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
