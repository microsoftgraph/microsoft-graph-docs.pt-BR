---
title: Tipo de recurso attachmentBase
description: Representa um tipo base abstrato para um anexo.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 355492402cd8532098ef81618c6407c0ba7f167a
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645594"
---
# <a name="attachmentbase-resource-type"></a>Tipo de recurso attachmentBase

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo base abstrato para um anexo. Você pode adicionar conteúdo relacionado a [um todoTask](../resources/todotask.md) na forma de um anexo.

Tipo base [de taskFileAttachment](../resources/taskfileattachment.md).

Herda de [entidade](../resources/entity.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentType|String|O tipo MIME.|
|id|Cadeia de caracteres|Identificador exclusivo do anexo. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|nome|Cadeia de caracteres|O nome de exibição do anexo. Não precisa ser o nome real do arquivo.|
|size|Int32|O comprimento do anexo em bytes.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachmentBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentBase",
  "contentType": "String",  
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": "Int32"
}
```

