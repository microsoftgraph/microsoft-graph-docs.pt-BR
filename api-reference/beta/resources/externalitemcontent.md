---
title: tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 66e3fccc8c072d06d2328301100d6bf3a0d50806
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777624"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="62b06-103">tipo de recurso externalItemContent</span><span class="sxs-lookup"><span data-stu-id="62b06-103">externalItemContent resource type</span></span>

<span data-ttu-id="62b06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62b06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62b06-105">O conteúdo de um [externalItem](externalitem.md) indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="62b06-105">The content of an [externalItem](externalitem.md) indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="62b06-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62b06-106">Properties</span></span>

| <span data-ttu-id="62b06-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62b06-107">Property</span></span> | <span data-ttu-id="62b06-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="62b06-108">Type</span></span>   | <span data-ttu-id="62b06-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62b06-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="62b06-110">valor</span><span class="sxs-lookup"><span data-stu-id="62b06-110">value</span></span>    | <span data-ttu-id="62b06-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62b06-111">String</span></span> | <span data-ttu-id="62b06-112">O conteúdo do externalItem.</span><span class="sxs-lookup"><span data-stu-id="62b06-112">The content for the externalItem.</span></span> <span data-ttu-id="62b06-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62b06-113">Required.</span></span>                                                 |
| <span data-ttu-id="62b06-114">type</span><span class="sxs-lookup"><span data-stu-id="62b06-114">type</span></span>     | <span data-ttu-id="62b06-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62b06-115">String</span></span> | <span data-ttu-id="62b06-116">O tipo de conteúdo na propriedade Value.</span><span class="sxs-lookup"><span data-stu-id="62b06-116">The type of content in the value property.</span></span> <span data-ttu-id="62b06-117">Os valores possíveis são: `text` e `html`.</span><span class="sxs-lookup"><span data-stu-id="62b06-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="62b06-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62b06-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="62b06-119">Relações</span><span class="sxs-lookup"><span data-stu-id="62b06-119">Relationships</span></span>

<span data-ttu-id="62b06-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62b06-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62b06-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62b06-121">JSON representation</span></span>

<span data-ttu-id="62b06-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62b06-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent"
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->


