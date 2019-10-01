---
title: pendingContentUpdate
description: O recurso pendingContentUpdate indica que uma operação que pode afetar o conteúdo binário do driveItem está aguardando a conclusão.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1637ac3faa1d42cd47f49735a1b24fb60868a23d
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333383"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="4d547-103">tipo de recurso pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="4d547-103">pendingContentUpdate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d547-104">Indica que uma operação que pode afetar o conteúdo binário do **driveItem** está aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="4d547-104">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="4d547-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d547-105">Properties</span></span>

| <span data-ttu-id="4d547-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d547-106">Property</span></span>     | <span data-ttu-id="4d547-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d547-107">Type</span></span>         | <span data-ttu-id="4d547-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d547-108">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="4d547-109">queuedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d547-109">queuedDateTime</span></span>|<span data-ttu-id="4d547-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d547-110">DateTimeOffset</span></span>|<span data-ttu-id="4d547-111">Data e hora em que a operação binária pendente foi enfileirada no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4d547-111">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="4d547-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4d547-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d547-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d547-113">JSON representation</span></span>

<span data-ttu-id="4d547-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d547-114">The following is a JSON representation of the resource.</span></span>

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
