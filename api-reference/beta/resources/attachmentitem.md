---
title: tipo de recurso attachmentItem
description: Representa os atributos de um item a ser anexado.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 14213afcaf555b21816a3b3ccf2481c1555c4b90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040172"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="95871-103">tipo de recurso attachmentItem</span><span class="sxs-lookup"><span data-stu-id="95871-103">attachmentItem resource type</span></span>

<span data-ttu-id="95871-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95871-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95871-105">Representa os atributos de um item a ser anexado.</span><span class="sxs-lookup"><span data-stu-id="95871-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="95871-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95871-106">Properties</span></span>

| <span data-ttu-id="95871-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95871-107">Property</span></span>     | <span data-ttu-id="95871-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="95871-108">Type</span></span>        | <span data-ttu-id="95871-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="95871-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95871-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="95871-110">attachmentType</span></span>|<span data-ttu-id="95871-111">String</span><span class="sxs-lookup"><span data-stu-id="95871-111">String</span></span>| <span data-ttu-id="95871-112">O tipo de anexo.</span><span class="sxs-lookup"><span data-stu-id="95871-112">The type of attachment.</span></span> <span data-ttu-id="95871-113">Os valores possíveis são: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="95871-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="95871-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95871-114">Required.</span></span>|
|<span data-ttu-id="95871-115">contentType</span><span class="sxs-lookup"><span data-stu-id="95871-115">contentType</span></span>|<span data-ttu-id="95871-116">String</span><span class="sxs-lookup"><span data-stu-id="95871-116">String</span></span>|<span data-ttu-id="95871-117">A natureza dos dados no anexo.</span><span class="sxs-lookup"><span data-stu-id="95871-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="95871-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="95871-118">Optional.</span></span>|
|<span data-ttu-id="95871-119">isInline</span><span class="sxs-lookup"><span data-stu-id="95871-119">isInline</span></span>|<span data-ttu-id="95871-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="95871-120">Boolean</span></span>|<span data-ttu-id="95871-121">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="95871-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="95871-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="95871-122">Optional.</span></span>|
|<span data-ttu-id="95871-123">nome</span><span class="sxs-lookup"><span data-stu-id="95871-123">name</span></span>|<span data-ttu-id="95871-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95871-124">String</span></span>|<span data-ttu-id="95871-125">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="95871-125">The display name of the attachment.</span></span> <span data-ttu-id="95871-126">Pode ser uma cadeia de caracteres descritiva e não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="95871-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="95871-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95871-127">Required.</span></span>|
|<span data-ttu-id="95871-128">size</span><span class="sxs-lookup"><span data-stu-id="95871-128">size</span></span>|<span data-ttu-id="95871-129">Int64</span><span class="sxs-lookup"><span data-stu-id="95871-129">Int64</span></span>|<span data-ttu-id="95871-130">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="95871-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="95871-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95871-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95871-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95871-132">JSON representation</span></span>

<span data-ttu-id="95871-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95871-133">The following is a JSON representation of the resource.</span></span>

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

