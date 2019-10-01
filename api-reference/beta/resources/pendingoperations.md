---
title: pendingOperations
description: O recurso pendingOperations indica que uma ou mais operações que podem afetar o estado do driveItem estão aguardando a conclusão.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d83a68bf555fa5cc239fb38b147d12754f223e13
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333382"
---
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="79a44-103">tipo de recurso pendingOperations</span><span class="sxs-lookup"><span data-stu-id="79a44-103">pendingOperations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79a44-104">Indica que uma ou mais operações que podem afetar o estado de **driveItem** estão aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="79a44-104">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="79a44-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79a44-105">Properties</span></span>

| <span data-ttu-id="79a44-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79a44-106">Property</span></span>     | <span data-ttu-id="79a44-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="79a44-107">Type</span></span>        | <span data-ttu-id="79a44-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="79a44-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79a44-109">pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="79a44-109">pendingContentUpdate</span></span>|[<span data-ttu-id="79a44-110">pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="79a44-110">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="79a44-111">Uma propriedade que indica que uma operação que pode atualizar o conteúdo binário de um arquivo está aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="79a44-111">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79a44-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79a44-112">JSON representation</span></span>

<span data-ttu-id="79a44-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79a44-113">The following is a JSON representation of the resource.</span></span>

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
