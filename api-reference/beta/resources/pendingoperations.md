---
title: pendingOperations
description: O recurso pendingOperations indica que uma ou mais operações que podem afetar o estado do driveItem estão pendentes de conclusão.
ms.localizationpriority: medium
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 6cf3903a99405dbcbdf83f26da053030e46dbb9e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176534"
---
# <a name="pendingoperations-resource-type"></a>Tipo de recurso pendingOperations

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica que uma ou mais operações que podem afetar o estado do **driveItem** estão pendentes de conclusão.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|pendingContentUpdate|[pendingContentUpdate](pendingcontentupdate.md)|Uma propriedade que indica que uma operação que pode atualizar o conteúdo binário de um arquivo está com a conclusão pendente.|

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


