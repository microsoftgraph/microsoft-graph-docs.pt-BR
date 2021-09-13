---
title: pendingContentUpdate
description: O recurso pendingContentUpdate indica que uma operação que pode afetar o conteúdo binário do driveItem está pendente de conclusão.
ms.localizationpriority: medium
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: d472ba41c26885bdefad13f35ea66f7b4e974d6a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117929"
---
# <a name="pendingcontentupdate-resource-type"></a>Tipo de recurso pendingContentUpdate

Namespace: microsoft.graph

Indica que uma operação que pode afetar o conteúdo binário do **driveItem** está pendente de conclusão.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo         | Descrição |
|:-------------|:-------------|:------------|
|**queuedDateTime**|DateTimeOffset|Data e hora em que a operação binária pendente foi en fila no horário UTC. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->

