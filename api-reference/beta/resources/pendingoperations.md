---
title: pendingOperations
description: O recurso pendingOperations indica que uma ou mais operações que podem afetar o estado do driveItem estão aguardando a conclusão.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 31629ee29bc91b3b2bae53e954743df17cde7d30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521966"
---
# <a name="pendingoperations-resource-type"></a><span data-ttu-id="9451e-103">tipo de recurso pendingOperations</span><span class="sxs-lookup"><span data-stu-id="9451e-103">pendingOperations resource type</span></span>

<span data-ttu-id="9451e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9451e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9451e-105">Indica que uma ou mais operações que podem afetar o estado de **driveItem** estão aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="9451e-105">Indicates that one or more operations that might affect the state of the **driveItem** are pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="9451e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9451e-106">Properties</span></span>

| <span data-ttu-id="9451e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9451e-107">Property</span></span>     | <span data-ttu-id="9451e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9451e-108">Type</span></span>        | <span data-ttu-id="9451e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9451e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9451e-110">pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="9451e-110">pendingContentUpdate</span></span>|[<span data-ttu-id="9451e-111">pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="9451e-111">pendingContentUpdate</span></span>](pendingcontentupdate.md)|<span data-ttu-id="9451e-112">Uma propriedade que indica que uma operação que pode atualizar o conteúdo binário de um arquivo está aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="9451e-112">A property that indicates that an operation that might update the binary content of a file is pending completion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9451e-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9451e-113">JSON representation</span></span>

<span data-ttu-id="9451e-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9451e-114">The following is a JSON representation of the resource.</span></span>

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
