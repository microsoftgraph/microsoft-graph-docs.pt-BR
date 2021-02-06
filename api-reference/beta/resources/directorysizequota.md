---
title: Tipo de recurso directorySizeQuota
description: Representa a cota de diretório total e usada de uma empresa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 3af82a957e152f0edf4d87e6fdf9a7888d4b64e4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133984"
---
# <a name="directorysizequota-resource-type"></a><span data-ttu-id="d3917-103">Tipo de recurso directorySizeQuota</span><span class="sxs-lookup"><span data-stu-id="d3917-103">directorySizeQuota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3917-104">Representa a cota de diretório total e usada de uma empresa.</span><span class="sxs-lookup"><span data-stu-id="d3917-104">Represents a company's used and total directory quota.</span></span>

## <a name="properties"></a><span data-ttu-id="d3917-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3917-105">Properties</span></span>
| <span data-ttu-id="d3917-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3917-106">Property</span></span>   | <span data-ttu-id="d3917-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3917-107">Type</span></span>|<span data-ttu-id="d3917-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3917-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3917-109">usado</span><span class="sxs-lookup"><span data-stu-id="d3917-109">used</span></span>|<span data-ttu-id="d3917-110">Int32</span><span class="sxs-lookup"><span data-stu-id="d3917-110">Int32</span></span>| <span data-ttu-id="d3917-111">Quantidade usada da cota de diretório.</span><span class="sxs-lookup"><span data-stu-id="d3917-111">Used amount of the directory quota.</span></span> |
|<span data-ttu-id="d3917-112">total</span><span class="sxs-lookup"><span data-stu-id="d3917-112">total</span></span>|<span data-ttu-id="d3917-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d3917-113">Int32</span></span>| <span data-ttu-id="d3917-114">Valor total da cota de diretório.</span><span class="sxs-lookup"><span data-stu-id="d3917-114">Total amount of the directory quota.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3917-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3917-115">JSON representation</span></span>

<span data-ttu-id="d3917-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3917-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
