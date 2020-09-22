---
title: tipo de recurso FileHash
description: Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 06097280b54e065842db7aa53ff060ce2ce5d5e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986082"
---
# <a name="filehash-resource-type"></a>tipo de recurso FileHash

Namespace: microsoft.graph

Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hashtype|Enumeração [Filehashtype](filehashtypeenumtype.md)|Tipo de hash de arquivo. Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.|
|hashValue|String|Valor do hash do arquivo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


