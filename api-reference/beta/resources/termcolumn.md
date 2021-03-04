---
author: swapnil1993
title: Tipo de recurso termColumn
description: O recurso termColumn indica que os valores da coluna contêm dados de taxonomia.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6d29ec570d7f3fad798fb1e2ba213b5a998643dc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445923"
---
# <a name="termcolumn-resource-type"></a><span data-ttu-id="231d3-103">Tipo de recurso termColumn</span><span class="sxs-lookup"><span data-stu-id="231d3-103">termColumn resource type</span></span>

<span data-ttu-id="231d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="231d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="231d3-105">Indica que os valores da coluna contêm dados de taxonomia.</span><span class="sxs-lookup"><span data-stu-id="231d3-105">Indicates that the column's values contains taxonomy data.</span></span>

## <a name="properties"></a><span data-ttu-id="231d3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="231d3-106">Properties</span></span>

| <span data-ttu-id="231d3-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="231d3-107">Property name</span></span> | <span data-ttu-id="231d3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="231d3-108">Type</span></span>   | <span data-ttu-id="231d3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="231d3-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="231d3-110">allowMultipleValues</span><span class="sxs-lookup"><span data-stu-id="231d3-110">allowMultipleValues</span></span> | <span data-ttu-id="231d3-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="231d3-111">Boolean</span></span> | <span data-ttu-id="231d3-112">Especifica se a coluna permitirá mais de um valor</span><span class="sxs-lookup"><span data-stu-id="231d3-112">Specifies whether the column will allow more than one value</span></span>   
| <span data-ttu-id="231d3-113">parentTerm</span><span class="sxs-lookup"><span data-stu-id="231d3-113">parentTerm</span></span>     | <span data-ttu-id="231d3-114">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="231d3-114">microsoft.graph.termStore.term</span></span> | <span data-ttu-id="231d3-115">Especifica o guid do termo cujos filhos podem ser selecionados como o valor da coluna.</span><span class="sxs-lookup"><span data-stu-id="231d3-115">Specifies the term guid whose children can be selected as column's value.</span></span>  
| <span data-ttu-id="231d3-116">showFullyQualifiedName</span><span class="sxs-lookup"><span data-stu-id="231d3-116">showFullyQualifiedName</span></span> | <span data-ttu-id="231d3-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="231d3-117">Boolean</span></span> | <span data-ttu-id="231d3-118">Especifica se o caminho do termo inteiro será exibido ou somente o rótulo do termo.</span><span class="sxs-lookup"><span data-stu-id="231d3-118">Specifies whether to display the entire term path or only the term label.</span></span>  
| <span data-ttu-id="231d3-119">termSet</span><span class="sxs-lookup"><span data-stu-id="231d3-119">termSet</span></span>      | <span data-ttu-id="231d3-120">microsoft.graph.termStore.set</span><span class="sxs-lookup"><span data-stu-id="231d3-120">microsoft.graph.termStore.set</span></span> | <span data-ttu-id="231d3-121">Termset cujos filhos podem ser selecionados como o valor da coluna.</span><span class="sxs-lookup"><span data-stu-id="231d3-121">Termset whose children can be selected as column's value.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="231d3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="231d3-122">JSON representation</span></span>

<span data-ttu-id="231d3-123">Aqui está uma representação JSON de um **recurso termColumn.**</span><span class="sxs-lookup"><span data-stu-id="231d3-123">Here is a JSON representation of a **termColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```

