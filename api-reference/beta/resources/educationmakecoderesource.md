---
title: tipo de recurso educationMakeCodeResource
description: Um recurso MakeCode
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5ffab7e11675996e79aed746cfe4624b28e37aab
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418283"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="c8d9b-103">tipo de recurso educationMakeCodeResource</span><span class="sxs-lookup"><span data-stu-id="c8d9b-103">educationMakeCodeResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8d9b-104">Um recurso representando um projeto [MakeCode](https://www.microsoft.com/en-us/makecode) .</span><span class="sxs-lookup"><span data-stu-id="c8d9b-104">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="c8d9b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8d9b-105">Properties</span></span>

| <span data-ttu-id="c8d9b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8d9b-106">Property</span></span>     | <span data-ttu-id="c8d9b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8d9b-107">Type</span></span>        | <span data-ttu-id="c8d9b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8d9b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c8d9b-109">projectId</span><span class="sxs-lookup"><span data-stu-id="c8d9b-109">projectId</span></span>|<span data-ttu-id="c8d9b-110">String</span><span class="sxs-lookup"><span data-stu-id="c8d9b-110">String</span></span>|<span data-ttu-id="c8d9b-111">ID do projeto MakeCode</span><span class="sxs-lookup"><span data-stu-id="c8d9b-111">ID of the MakeCode project</span></span>|
|<span data-ttu-id="c8d9b-112">hostWebUrl</span><span class="sxs-lookup"><span data-stu-id="c8d9b-112">hostWebUrl</span></span>|<span data-ttu-id="c8d9b-113">String</span><span class="sxs-lookup"><span data-stu-id="c8d9b-113">String</span></span>|<span data-ttu-id="c8d9b-114">Host para o tipo de recurso MakeCode (por exemplo,, MICROBIT)</span><span class="sxs-lookup"><span data-stu-id="c8d9b-114">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8d9b-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8d9b-115">JSON representation</span></span>

<span data-ttu-id="c8d9b-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8d9b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "projectId": "String",
  "hostWebUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->