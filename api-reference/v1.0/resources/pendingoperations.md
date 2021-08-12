---
title: pendingOperations
description: O recurso pendingOperations indica que uma ou mais operações que podem afetar o estado do driveItem estão pendentes de conclusão.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 8fac755c6bcce65af03a96b1c13d6186ae3c1f86e975cf9577d0a5e568ebe62a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178116"
---
# <a name="pendingoperations-resource-type"></a>Tipo de recurso pendingOperations

Namespace: microsoft.graph

Indica que uma ou mais operações que podem afetar o estado do **driveItem** estão pendentes de conclusão.

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo        | Descrição |
|:------------------------|:------------|:------------|
|**pendingContentUpdate** |[pendingContentUpdate](pendingcontentupdate.md)|Uma propriedade que indica que uma operação que pode atualizar o conteúdo binário de um arquivo está pendente de conclusão.|

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

