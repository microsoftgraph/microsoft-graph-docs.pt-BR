---
title: tipo de recurso attachmentItem
description: Representa os atributos de um item a ser anexado.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5df3abd262ae9b09fa1843648906c70d07e6ec51
ms.sourcegitcommit: feebe30e62aa19ce5cb8e8338e043326e464ed9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991853"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="1bd84-103">tipo de recurso attachmentItem</span><span class="sxs-lookup"><span data-stu-id="1bd84-103">attachmentItem resource type</span></span>

<span data-ttu-id="1bd84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd84-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bd84-105">Representa os atributos de um item a ser anexado.</span><span class="sxs-lookup"><span data-stu-id="1bd84-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="1bd84-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bd84-106">Properties</span></span>

| <span data-ttu-id="1bd84-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bd84-107">Property</span></span>     | <span data-ttu-id="1bd84-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bd84-108">Type</span></span>        | <span data-ttu-id="1bd84-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bd84-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1bd84-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="1bd84-110">attachmentType</span></span>|<span data-ttu-id="1bd84-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1bd84-111">String</span></span>| <span data-ttu-id="1bd84-112">O tipo de anexo.</span><span class="sxs-lookup"><span data-stu-id="1bd84-112">The type of attachment.</span></span> <span data-ttu-id="1bd84-113">Os valores possíveis são: `file`, `item`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="1bd84-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="1bd84-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bd84-114">Required.</span></span>|
|<span data-ttu-id="1bd84-115">contentType</span><span class="sxs-lookup"><span data-stu-id="1bd84-115">contentType</span></span>|<span data-ttu-id="1bd84-116">String</span><span class="sxs-lookup"><span data-stu-id="1bd84-116">String</span></span>|<span data-ttu-id="1bd84-117">A natureza dos dados no anexo.</span><span class="sxs-lookup"><span data-stu-id="1bd84-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="1bd84-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1bd84-118">Optional.</span></span>|
|<span data-ttu-id="1bd84-119">isInline</span><span class="sxs-lookup"><span data-stu-id="1bd84-119">isInline</span></span>|<span data-ttu-id="1bd84-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bd84-120">Boolean</span></span>|<span data-ttu-id="1bd84-121">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="1bd84-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="1bd84-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1bd84-122">Optional.</span></span>|
|<span data-ttu-id="1bd84-123">name</span><span class="sxs-lookup"><span data-stu-id="1bd84-123">name</span></span>|<span data-ttu-id="1bd84-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bd84-124">String</span></span>|<span data-ttu-id="1bd84-125">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="1bd84-125">The display name of the attachment.</span></span> <span data-ttu-id="1bd84-126">Pode ser uma cadeia de caracteres descritiva e não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="1bd84-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="1bd84-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bd84-127">Required.</span></span>|
|<span data-ttu-id="1bd84-128">size</span><span class="sxs-lookup"><span data-stu-id="1bd84-128">size</span></span>|<span data-ttu-id="1bd84-129">Int64</span><span class="sxs-lookup"><span data-stu-id="1bd84-129">Int64</span></span>|<span data-ttu-id="1bd84-130">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="1bd84-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="1bd84-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bd84-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1bd84-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bd84-132">JSON representation</span></span>

<span data-ttu-id="1bd84-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bd84-133">The following is a JSON representation of the resource.</span></span>

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