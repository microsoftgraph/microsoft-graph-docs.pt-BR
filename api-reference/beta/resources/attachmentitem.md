---
title: tipo de recurso attachmentItem
description: Representa os atributos de um item a ser anexado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b6570b44bab06c0ab4b8b6788ea585276b43c3cc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621635"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="17d59-103">tipo de recurso attachmentItem</span><span class="sxs-lookup"><span data-stu-id="17d59-103">attachmentItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17d59-104">Representa os atributos de um item a ser anexado.</span><span class="sxs-lookup"><span data-stu-id="17d59-104">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="17d59-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17d59-105">Properties</span></span>

| <span data-ttu-id="17d59-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17d59-106">Property</span></span>     | <span data-ttu-id="17d59-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="17d59-107">Type</span></span>        | <span data-ttu-id="17d59-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="17d59-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17d59-109">attachmentType</span><span class="sxs-lookup"><span data-stu-id="17d59-109">attachmentType</span></span>|<span data-ttu-id="17d59-110">String</span><span class="sxs-lookup"><span data-stu-id="17d59-110">String</span></span>| <span data-ttu-id="17d59-111">O tipo de anexo.</span><span class="sxs-lookup"><span data-stu-id="17d59-111">The type of attachment.</span></span> <span data-ttu-id="17d59-112">Os valores possíveis são: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="17d59-112">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="17d59-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17d59-113">Required.</span></span>|
|<span data-ttu-id="17d59-114">contentType</span><span class="sxs-lookup"><span data-stu-id="17d59-114">contentType</span></span>|<span data-ttu-id="17d59-115">String</span><span class="sxs-lookup"><span data-stu-id="17d59-115">String</span></span>|<span data-ttu-id="17d59-116">A natureza dos dados no anexo.</span><span class="sxs-lookup"><span data-stu-id="17d59-116">The nature of the data in the attachment.</span></span> <span data-ttu-id="17d59-117">Opcional.</span><span class="sxs-lookup"><span data-stu-id="17d59-117">Optional.</span></span>|
|<span data-ttu-id="17d59-118">isInline</span><span class="sxs-lookup"><span data-stu-id="17d59-118">isInline</span></span>|<span data-ttu-id="17d59-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="17d59-119">Boolean</span></span>|<span data-ttu-id="17d59-120">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="17d59-120">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="17d59-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="17d59-121">Optional.</span></span>|
|<span data-ttu-id="17d59-122">name</span><span class="sxs-lookup"><span data-stu-id="17d59-122">name</span></span>|<span data-ttu-id="17d59-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17d59-123">String</span></span>|<span data-ttu-id="17d59-124">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="17d59-124">The display name of the attachment.</span></span> <span data-ttu-id="17d59-125">Pode ser uma cadeia de caracteres descritiva e não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="17d59-125">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="17d59-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17d59-126">Required.</span></span>|
|<span data-ttu-id="17d59-127">size</span><span class="sxs-lookup"><span data-stu-id="17d59-127">size</span></span>|<span data-ttu-id="17d59-128">Int64</span><span class="sxs-lookup"><span data-stu-id="17d59-128">Int64</span></span>|<span data-ttu-id="17d59-129">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="17d59-129">The length of the attachment in bytes.</span></span> <span data-ttu-id="17d59-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17d59-130">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17d59-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17d59-131">JSON representation</span></span>

<span data-ttu-id="17d59-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17d59-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
  "contentType": "String",
  "isInline": true,
  "name": "String",
  "size": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachmentItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->