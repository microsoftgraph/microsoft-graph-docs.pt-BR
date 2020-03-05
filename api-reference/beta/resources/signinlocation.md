---
title: tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a entrada ocorreu.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: fbe356cf939236e1965a2a7005d791bc3a814acc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520580"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="a0dca-103">tipo de recurso signInLocation</span><span class="sxs-lookup"><span data-stu-id="a0dca-103">signInLocation resource type</span></span>

<span data-ttu-id="a0dca-104">Namespace: o Microsoft. Graph fornece a cidade, o estado e o país/região de onde a entrada ocorreu.</span><span class="sxs-lookup"><span data-stu-id="a0dca-104">Namespace: microsoft.graph Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="a0dca-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0dca-105">Properties</span></span>
| <span data-ttu-id="a0dca-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0dca-106">Property</span></span>     | <span data-ttu-id="a0dca-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0dca-107">Type</span></span>   |<span data-ttu-id="a0dca-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0dca-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0dca-109">city</span><span class="sxs-lookup"><span data-stu-id="a0dca-109">city</span></span>|<span data-ttu-id="a0dca-110">String</span><span class="sxs-lookup"><span data-stu-id="a0dca-110">String</span></span>|<span data-ttu-id="a0dca-111">Fornece a cidade onde a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="a0dca-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="a0dca-112">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="a0dca-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="a0dca-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a0dca-113">countryOrRegion</span></span>|<span data-ttu-id="a0dca-114">String</span><span class="sxs-lookup"><span data-stu-id="a0dca-114">String</span></span>|<span data-ttu-id="a0dca-115">Fornece as informações do código do país (código de 2 letras) em que a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="a0dca-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="a0dca-116">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="a0dca-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="a0dca-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a0dca-117">geoCoordinates</span></span>|[<span data-ttu-id="a0dca-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a0dca-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="a0dca-119">Fornece a latitude, longitude e altitude onde a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="a0dca-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="a0dca-120">state</span><span class="sxs-lookup"><span data-stu-id="a0dca-120">state</span></span>|<span data-ttu-id="a0dca-121">String</span><span class="sxs-lookup"><span data-stu-id="a0dca-121">String</span></span>|<span data-ttu-id="a0dca-122">Fornece o estado em que a entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="a0dca-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="a0dca-123">Isso é calculado usando informações de latitude/longitude da atividade de entrada.</span><span class="sxs-lookup"><span data-stu-id="a0dca-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0dca-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0dca-124">JSON representation</span></span>

<span data-ttu-id="a0dca-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0dca-125">Here is a JSON representation of the resource.</span></span>

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
