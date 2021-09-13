---
title: Tipo de recurso educationFileResource
description: Uma subclasse de educationResource que representa um objeto de arquivo associado à atribuição ou envio.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e0e101e1d21bd8e5aa205875a9f444678aeee218
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036638"
---
# <a name="educationfileresource-resource-type"></a>Tipo de recurso educationFileResource

Namespace: microsoft.graph

Uma subclasse [de educationResource](educationresource.md) que representa um objeto de arquivo associado à atribuição ou envio.

Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem tratamento especial dentro do sistema. O recurso de arquivo deve ser armazenado no **resourceFolder** que está associado à atribuição ou ao envio ao que esse recurso está anexado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fileUrl|Cadeia de caracteres|Local no disco do recurso de arquivo.|

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


