---
title: tipo de recurso FileHash
description: Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c82632658e4936ecae812f6bdf1826ad6120d2d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532955"
---
# <a name="filehash-resource-type"></a>tipo de recurso FileHash

Namespace: microsoft.graph

Contém informações com monitoração de hash de arquivo (criptografia e confidencialidade de local).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hashtype|fileHashType|Tipo de hash de arquivo. Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.|
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
