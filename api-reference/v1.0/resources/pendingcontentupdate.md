---
title: pendingContentUpdate
description: O recurso pendingContentUpdate indica que uma operação que pode afetar o conteúdo binário do driveItem está aguardando a conclusão.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: b1a197ae60dc8bb60533d567c6472a65988c3962
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863800"
---
# <a name="pendingcontentupdate-resource-type"></a>tipo de recurso pendingContentUpdate

Namespace: microsoft.graph

Indica que uma operação que pode afetar o conteúdo binário do **driveItem** está aguardando a conclusão.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo         | Descrição |
|:-------------|:-------------|:------------|
|**queuedDateTime**|DateTimeOffset|Data e hora em que a operação binária pendente foi enfileirada no horário UTC. Somente leitura.|

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
