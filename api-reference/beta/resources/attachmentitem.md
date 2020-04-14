---
title: tipo de recurso attachmentItem
description: Representa os atributos de um item a ser anexado.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7402a22665fec8716156395f4a783c804a42febb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461020"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="ff2c0-103">tipo de recurso attachmentItem</span><span class="sxs-lookup"><span data-stu-id="ff2c0-103">attachmentItem resource type</span></span>

<span data-ttu-id="ff2c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff2c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff2c0-105">Representa os atributos de um item a ser anexado.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="ff2c0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff2c0-106">Properties</span></span>

| <span data-ttu-id="ff2c0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff2c0-107">Property</span></span>     | <span data-ttu-id="ff2c0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff2c0-108">Type</span></span>        | <span data-ttu-id="ff2c0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff2c0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff2c0-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="ff2c0-110">attachmentType</span></span>|<span data-ttu-id="ff2c0-111">String</span><span class="sxs-lookup"><span data-stu-id="ff2c0-111">String</span></span>| <span data-ttu-id="ff2c0-112">O tipo de anexo.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-112">The type of attachment.</span></span> <span data-ttu-id="ff2c0-113">Os valores possíveis são: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="ff2c0-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-114">Required.</span></span>|
|<span data-ttu-id="ff2c0-115">contentType</span><span class="sxs-lookup"><span data-stu-id="ff2c0-115">contentType</span></span>|<span data-ttu-id="ff2c0-116">String</span><span class="sxs-lookup"><span data-stu-id="ff2c0-116">String</span></span>|<span data-ttu-id="ff2c0-117">A natureza dos dados no anexo.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="ff2c0-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-118">Optional.</span></span>|
|<span data-ttu-id="ff2c0-119">isInline</span><span class="sxs-lookup"><span data-stu-id="ff2c0-119">isInline</span></span>|<span data-ttu-id="ff2c0-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff2c0-120">Boolean</span></span>|<span data-ttu-id="ff2c0-121">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="ff2c0-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-122">Optional.</span></span>|
|<span data-ttu-id="ff2c0-123">nome</span><span class="sxs-lookup"><span data-stu-id="ff2c0-123">name</span></span>|<span data-ttu-id="ff2c0-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff2c0-124">String</span></span>|<span data-ttu-id="ff2c0-125">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-125">The display name of the attachment.</span></span> <span data-ttu-id="ff2c0-126">Pode ser uma cadeia de caracteres descritiva e não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="ff2c0-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-127">Required.</span></span>|
|<span data-ttu-id="ff2c0-128">size</span><span class="sxs-lookup"><span data-stu-id="ff2c0-128">size</span></span>|<span data-ttu-id="ff2c0-129">Int64</span><span class="sxs-lookup"><span data-stu-id="ff2c0-129">Int64</span></span>|<span data-ttu-id="ff2c0-130">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="ff2c0-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff2c0-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff2c0-132">JSON representation</span></span>

<span data-ttu-id="ff2c0-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff2c0-133">The following is a JSON representation of the resource.</span></span>

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