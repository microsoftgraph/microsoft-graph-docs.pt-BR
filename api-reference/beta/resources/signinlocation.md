---
title: tipo de recurso de signInLocation
description: Fornece a cidade, estado e país/região de onde a entrar aconteceu.
localization_priority: Normal
ms.openlocfilehash: 49d6dfb07c635ac3754b3e873d75911a43593a73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839134"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="bccc7-103">tipo de recurso de signInLocation</span><span class="sxs-lookup"><span data-stu-id="bccc7-103">signInLocation resource type</span></span>
<span data-ttu-id="bccc7-104">Fornece a cidade, estado e país/região de onde a entrar aconteceu.</span><span class="sxs-lookup"><span data-stu-id="bccc7-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="bccc7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bccc7-105">Properties</span></span>
| <span data-ttu-id="bccc7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bccc7-106">Property</span></span>     | <span data-ttu-id="bccc7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bccc7-107">Type</span></span>   |<span data-ttu-id="bccc7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bccc7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bccc7-109">city</span><span class="sxs-lookup"><span data-stu-id="bccc7-109">city</span></span>|<span data-ttu-id="bccc7-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bccc7-110">String</span></span>|<span data-ttu-id="bccc7-111">Fornece a cidade onde o sign-in se originou.</span><span class="sxs-lookup"><span data-stu-id="bccc7-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="bccc7-112">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="bccc7-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="bccc7-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="bccc7-113">countryOrRegion</span></span>|<span data-ttu-id="bccc7-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bccc7-114">String</span></span>|<span data-ttu-id="bccc7-115">Fornece as informações de código de país (código de carta 2) onde o sign-in se originou.</span><span class="sxs-lookup"><span data-stu-id="bccc7-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="bccc7-116">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="bccc7-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="bccc7-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="bccc7-117">geoCoordinates</span></span>|[<span data-ttu-id="bccc7-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="bccc7-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="bccc7-119">Fornece o latitude, longitude e altitude onde a entrar se originou.</span><span class="sxs-lookup"><span data-stu-id="bccc7-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="bccc7-120">estado</span><span class="sxs-lookup"><span data-stu-id="bccc7-120">state</span></span>|<span data-ttu-id="bccc7-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bccc7-121">String</span></span>|<span data-ttu-id="bccc7-122">Fornece o estado em que a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="bccc7-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="bccc7-123">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="bccc7-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bccc7-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bccc7-124">JSON representation</span></span>

<span data-ttu-id="bccc7-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bccc7-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
