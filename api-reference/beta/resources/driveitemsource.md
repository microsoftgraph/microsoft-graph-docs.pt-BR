---
author: MarcMroz
description: O driveItemSource contém metadados sobre o aplicativo de origem em que o item de unidade foi criado.
title: Tipo de recurso driveItemSource
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: a403f570ac550b62f9c0e7fa0c3c2fa9758e1772
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236287"
---
# <a name="driveitemsource-resource-type"></a><span data-ttu-id="16aaa-103">Tipo de recurso driveItemSource</span><span class="sxs-lookup"><span data-stu-id="16aaa-103">driveItemSource resource type</span></span>

<span data-ttu-id="16aaa-104">Contém metadados sobre a origem do item de unidade.</span><span class="sxs-lookup"><span data-stu-id="16aaa-104">Contains metadata about the source of the drive item.</span></span>

<span data-ttu-id="16aaa-105">Ele está disponível na propriedade de origem dos [recursos driveItem.][item-resource]</span><span class="sxs-lookup"><span data-stu-id="16aaa-105">It is available on the source property of [driveItem][item-resource] resources.</span></span>

## <a name="properties"></a><span data-ttu-id="16aaa-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16aaa-106">Properties</span></span>

| <span data-ttu-id="16aaa-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16aaa-107">Property</span></span>                 | <span data-ttu-id="16aaa-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="16aaa-108">Type</span></span>                       | <span data-ttu-id="16aaa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="16aaa-109">Description</span></span>                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| <span data-ttu-id="16aaa-110">**application**</span><span class="sxs-lookup"><span data-stu-id="16aaa-110">**application**</span></span>          | <span data-ttu-id="16aaa-111">driveItemSourceApplication</span><span class="sxs-lookup"><span data-stu-id="16aaa-111">driveItemSourceApplication</span></span> | <span data-ttu-id="16aaa-112">Valor de enumeração que indica o aplicativo de origem onde o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="16aaa-112">Enumeration value that indicates the source application where the file was created.</span></span>              |
| <span data-ttu-id="16aaa-113">**externalId**</span><span class="sxs-lookup"><span data-stu-id="16aaa-113">**externalId**</span></span>           | <span data-ttu-id="16aaa-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16aaa-114">string</span></span>                     | <span data-ttu-id="16aaa-115">O identificador externo do item de unidade da fonte.</span><span class="sxs-lookup"><span data-stu-id="16aaa-115">The external identifier for the drive item from the source.</span></span>                                      |

### <a name="driveitemsourceapplication-values"></a><span data-ttu-id="16aaa-116">valores driveItemSourceApplication</span><span class="sxs-lookup"><span data-stu-id="16aaa-116">driveItemSourceApplication values</span></span>

| <span data-ttu-id="16aaa-117">Valor</span><span class="sxs-lookup"><span data-stu-id="16aaa-117">Value</span></span>               | <span data-ttu-id="16aaa-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="16aaa-118">Description</span></span>                                       |
|:--------------------|:--------------------------------------------------|
| <span data-ttu-id="16aaa-119">teams</span><span class="sxs-lookup"><span data-stu-id="16aaa-119">teams</span></span>               | <span data-ttu-id="16aaa-120">O aplicativo é Teams.</span><span class="sxs-lookup"><span data-stu-id="16aaa-120">The application is Teams.</span></span>                         |
| <span data-ttu-id="16aaa-121">yammer</span><span class="sxs-lookup"><span data-stu-id="16aaa-121">yammer</span></span>              | <span data-ttu-id="16aaa-122">O aplicativo é Yammer.</span><span class="sxs-lookup"><span data-stu-id="16aaa-122">The application is Yammer.</span></span>                        |
| <span data-ttu-id="16aaa-123">sharePoint</span><span class="sxs-lookup"><span data-stu-id="16aaa-123">sharePoint</span></span>          | <span data-ttu-id="16aaa-124">O aplicativo é SharePoint.</span><span class="sxs-lookup"><span data-stu-id="16aaa-124">The application is SharePoint.</span></span>                    |
| <span data-ttu-id="16aaa-125">oneDrive</span><span class="sxs-lookup"><span data-stu-id="16aaa-125">oneDrive</span></span>            | <span data-ttu-id="16aaa-126">O aplicativo é OneDrive.</span><span class="sxs-lookup"><span data-stu-id="16aaa-126">The application is OneDrive.</span></span>                      |
| <span data-ttu-id="16aaa-127">stream</span><span class="sxs-lookup"><span data-stu-id="16aaa-127">stream</span></span>              | <span data-ttu-id="16aaa-128">O aplicativo é Stream.</span><span class="sxs-lookup"><span data-stu-id="16aaa-128">The application is Stream.</span></span>                        |
| <span data-ttu-id="16aaa-129">powerPoint</span><span class="sxs-lookup"><span data-stu-id="16aaa-129">powerPoint</span></span>          | <span data-ttu-id="16aaa-130">O aplicativo é PowerPoint</span><span class="sxs-lookup"><span data-stu-id="16aaa-130">The application is PowerPoint</span></span>                     |
| <span data-ttu-id="16aaa-131">office</span><span class="sxs-lookup"><span data-stu-id="16aaa-131">office</span></span>              | <span data-ttu-id="16aaa-132">O aplicativo é Office</span><span class="sxs-lookup"><span data-stu-id="16aaa-132">The application is Office</span></span>                         |
| <span data-ttu-id="16aaa-133">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="16aaa-133">unknownFutureValue</span></span>  | <span data-ttu-id="16aaa-134">Valor do marcador para compatibilidade futura.</span><span class="sxs-lookup"><span data-stu-id="16aaa-134">Marker value for future compatibility.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="16aaa-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16aaa-135">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "application",
    "externalId",
  ],
  "@odata.type": "microsoft.graph.driveItemSource"
}-->

```json
{
  "application": "string",
  "externalId" : "string"
}
```

## <a name="see-also"></a><span data-ttu-id="16aaa-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="16aaa-136">See also</span></span>

<span data-ttu-id="16aaa-137">Para obter mais informações sobre as facetas em um driveItem, [consulte driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="16aaa-137">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The driveItemSource facet provides information about drive item source.",
  "keywords": "driveItemSoruce,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/driveItemSource"
} -->
