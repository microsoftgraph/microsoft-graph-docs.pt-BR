---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6c3dd1bdb565ce32e464e38d7909988b4f4c7791
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936280"
---
# <a name="location-resource-type"></a><span data-ttu-id="5515a-103">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="5515a-103">Location resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5515a-104">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="5515a-104">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="5515a-105">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="5515a-105">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="5515a-106">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="5515a-106">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="5515a-107">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="5515a-107">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="5515a-108">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="5515a-108">How event was created</span></span>  | <span data-ttu-id="5515a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5515a-109">Property</span></span>   | <span data-ttu-id="5515a-110">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="5515a-110">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="5515a-111">API REST [criar evento](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="5515a-111">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="5515a-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="5515a-112">**locationType**</span></span> | `default` |
| <span data-ttu-id="5515a-113">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="5515a-113">User interface in Outlook</span></span> | <span data-ttu-id="5515a-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="5515a-114">**locationType**</span></span> | <span data-ttu-id="5515a-115">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="5515a-115">One of the following:</span></span> <ul><li><span data-ttu-id="5515a-116">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="5515a-116">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="5515a-117">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="5515a-117">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="5515a-118">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="5515a-118">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="5515a-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5515a-119">Properties</span></span>
| <span data-ttu-id="5515a-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5515a-120">Property</span></span>  | <span data-ttu-id="5515a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5515a-121">Type</span></span>   | <span data-ttu-id="5515a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5515a-122">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="5515a-123">address</span><span class="sxs-lookup"><span data-stu-id="5515a-123">address</span></span> | [<span data-ttu-id="5515a-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5515a-124">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="5515a-125">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="5515a-125">The street address of the location.</span></span> |
| <span data-ttu-id="5515a-126">coordenadas</span><span class="sxs-lookup"><span data-stu-id="5515a-126">coordinates</span></span> | [<span data-ttu-id="5515a-127">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="5515a-127">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="5515a-128">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="5515a-128">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="5515a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="5515a-129">displayName</span></span>  | <span data-ttu-id="5515a-130">String</span><span class="sxs-lookup"><span data-stu-id="5515a-130">String</span></span> | <span data-ttu-id="5515a-131">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="5515a-131">The name associated with the location.</span></span>                       |
| <span data-ttu-id="5515a-132">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5515a-132">locationEmailAddress</span></span> | <span data-ttu-id="5515a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5515a-133">String</span></span> | <span data-ttu-id="5515a-134">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="5515a-134">Optional email address of the location.</span></span> |
| <span data-ttu-id="5515a-135">locationUri</span><span class="sxs-lookup"><span data-stu-id="5515a-135">locationUri</span></span> | <span data-ttu-id="5515a-136">String</span><span class="sxs-lookup"><span data-stu-id="5515a-136">String</span></span> | <span data-ttu-id="5515a-137">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="5515a-137">Optional URI representing the location.</span></span> |
| <span data-ttu-id="5515a-138">locationType</span><span class="sxs-lookup"><span data-stu-id="5515a-138">locationType</span></span> | <span data-ttu-id="5515a-139">locationType</span><span class="sxs-lookup"><span data-stu-id="5515a-139">locationType</span></span> | <span data-ttu-id="5515a-140">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="5515a-140">The type of location.</span></span> <span data-ttu-id="5515a-141">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="5515a-141">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="5515a-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5515a-142">Read-only.</span></span>|
| <span data-ttu-id="5515a-143">uniqueId</span><span class="sxs-lookup"><span data-stu-id="5515a-143">uniqueId</span></span> | <span data-ttu-id="5515a-144">String</span><span class="sxs-lookup"><span data-stu-id="5515a-144">String</span></span> | <span data-ttu-id="5515a-145">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="5515a-145">For internal use only.</span></span>|
| <span data-ttu-id="5515a-146">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="5515a-146">uniqueIdType</span></span> | <span data-ttu-id="5515a-147">String</span><span class="sxs-lookup"><span data-stu-id="5515a-147">String</span></span> | <span data-ttu-id="5515a-148">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="5515a-148">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="5515a-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5515a-149">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationType": "string",
  "locationUri": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/location.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
