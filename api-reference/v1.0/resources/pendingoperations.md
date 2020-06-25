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
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="a8108-103">tipo de recurso pendingOperations</span><span class="sxs-lookup"><span data-stu-id="a8108-103">pendingOperations resource type</span></span>

<span data-ttu-id="a8108-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8108-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8108-105">Indica que uma ou mais operações que podem afetar o estado de **driveItem** estão aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="a8108-105">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="a8108-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8108-106">Properties</span></span>

| <span data-ttu-id="a8108-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8108-107">Property</span></span>                | <span data-ttu-id="a8108-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8108-108">Type</span></span>        | <span data-ttu-id="a8108-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8108-109">Description</span></span> |
|:------------------------|:------------|:------------|
|<span data-ttu-id="a8108-110">**pendingContentUpdate**</span><span class="sxs-lookup"><span data-stu-id="a8108-110">**pendingContentUpdate**</span></span> |[<span data-ttu-id="a8108-111">pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="a8108-111">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="a8108-112">Uma propriedade que indica que uma operação que pode atualizar o conteúdo binário de um arquivo está aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="a8108-112">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8108-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8108-113">JSON representation</span></span>

<span data-ttu-id="a8108-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8108-114">The following is a JSON representation of the resource.</span></span>

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
