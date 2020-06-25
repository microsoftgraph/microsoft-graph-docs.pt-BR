---
title: pendingOperations
description: O recurso pendingOperations indica que uma ou mais operações que podem afetar o estado do driveItem estão aguardando a conclusão.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 381ecd3bf302a1e7d323211cac071e360340b5c6
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863681"
---
# <a name="pendingoperations-resource-type"></a>tipo de recurso pendingOperations

Namespace: microsoft.graph

Indica que uma ou mais operações que podem afetar o estado de **driveItem** estão aguardando a conclusão.

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo        | Descrição |
|:------------------------|:------------|:------------|
|**pendingContentUpdate** |[pendingContentUpdate](pendingcontentupdate.md)|Uma propriedade que indica que uma operação que pode atualizar o conteúdo binário de um arquivo está aguardando a conclusão.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingOperations",
  "baseType": null
}-->

```json
{
  "pendingContentUpdate": {"@odata.type": "microsoft.graph.pendingContentUpdate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingOperations resource indicates that an operation that may affect the state of the DriveItem is pending completion.",
  "keywords": "pendingoperations,pendingoperations,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->
