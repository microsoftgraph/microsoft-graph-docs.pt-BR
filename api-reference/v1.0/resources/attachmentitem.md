---
title: tipo de recurso attachmentItem
description: Representa os atributos de um item a ser anexado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 23ae9ed8371ecc4f49f6eb4b7fae5a14964cd15f
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591541"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="02260-103">tipo de recurso attachmentItem</span><span class="sxs-lookup"><span data-stu-id="02260-103">attachmentItem resource type</span></span>

<span data-ttu-id="02260-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02260-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02260-105">Representa os atributos de um item a ser anexado.</span><span class="sxs-lookup"><span data-stu-id="02260-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="02260-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02260-106">Properties</span></span>

| <span data-ttu-id="02260-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02260-107">Property</span></span>     | <span data-ttu-id="02260-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="02260-108">Type</span></span>        | <span data-ttu-id="02260-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="02260-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="02260-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="02260-110">attachmentType</span></span>|<span data-ttu-id="02260-111">String</span><span class="sxs-lookup"><span data-stu-id="02260-111">String</span></span>| <span data-ttu-id="02260-112">O tipo de anexo.</span><span class="sxs-lookup"><span data-stu-id="02260-112">The type of attachment.</span></span> <span data-ttu-id="02260-113">Os valores possíveis são: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="02260-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="02260-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02260-114">Required.</span></span>|
|<span data-ttu-id="02260-115">contentType</span><span class="sxs-lookup"><span data-stu-id="02260-115">contentType</span></span>|<span data-ttu-id="02260-116">String</span><span class="sxs-lookup"><span data-stu-id="02260-116">String</span></span>|<span data-ttu-id="02260-117">A natureza dos dados no anexo.</span><span class="sxs-lookup"><span data-stu-id="02260-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="02260-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02260-118">Optional.</span></span>|
|<span data-ttu-id="02260-119">isInline</span><span class="sxs-lookup"><span data-stu-id="02260-119">isInline</span></span>|<span data-ttu-id="02260-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="02260-120">Boolean</span></span>|<span data-ttu-id="02260-121">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="02260-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="02260-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02260-122">Optional.</span></span>|
|<span data-ttu-id="02260-123">name</span><span class="sxs-lookup"><span data-stu-id="02260-123">name</span></span>|<span data-ttu-id="02260-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02260-124">String</span></span>|<span data-ttu-id="02260-125">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="02260-125">The display name of the attachment.</span></span> <span data-ttu-id="02260-126">Pode ser uma cadeia de caracteres descritiva e não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="02260-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="02260-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02260-127">Required.</span></span>|
|<span data-ttu-id="02260-128">size</span><span class="sxs-lookup"><span data-stu-id="02260-128">size</span></span>|<span data-ttu-id="02260-129">Int64</span><span class="sxs-lookup"><span data-stu-id="02260-129">Int64</span></span>|<span data-ttu-id="02260-130">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="02260-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="02260-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02260-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02260-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02260-132">JSON representation</span></span>

<span data-ttu-id="02260-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02260-133">The following is a JSON representation of the resource.</span></span>

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