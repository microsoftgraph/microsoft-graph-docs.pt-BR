---
title: Tipo de recurso authoredNote
description: Representa as propriedades de uma nota escrita por um autor
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 30c635ada7a981a4a02c2a20b8904a02d5f24458
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446930"
---
# <a name="authorednote-resource-type"></a>Tipo de recurso authoredNote

Namespace: microsoft.graph

Representa as propriedades de uma nota escrita por um autor.

Herda da [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|autor|[identity](../resources/identity.md)|Informações de identidade sobre o autor da nota.|
|conteúdo|[itemBody](../resources/itembody.md)|O conteúdo da nota.|
|createdDateTime|DateTimeOffset|A data e a hora em que a entidade foi criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authoredNote",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authoredNote",
  "author": {
    "@odata.type": "microsoft.graph.identity"
  },
  "content": {
    "@odata.type": "microsoft.graph.itemBody",
    "content": "String",
    "contentType": "String"
  },
  "createdDateTime": "String (timestamp)"
}
```

