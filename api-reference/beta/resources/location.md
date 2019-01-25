---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
localization_priority: Normal
ms.openlocfilehash: 6e3c61bcf8f22a20bf41053c2310dc51f5b800a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508605"
---
# <a name="location-resource-type"></a><span data-ttu-id="f9414-103">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="f9414-103">Location resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9414-104">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="f9414-104">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="f9414-105">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f9414-105">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="f9414-106">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="f9414-106">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="f9414-107">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="f9414-107">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="f9414-108">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="f9414-108">How event was created</span></span>  | <span data-ttu-id="f9414-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9414-109">Property</span></span>   | <span data-ttu-id="f9414-110">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="f9414-110">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="f9414-111">API REST [criar evento](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="f9414-111">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="f9414-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="f9414-112">**locationType**</span></span> | `default` |
| <span data-ttu-id="f9414-113">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="f9414-113">User interface in Outlook</span></span> | <span data-ttu-id="f9414-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="f9414-114">**locationType**</span></span> | <span data-ttu-id="f9414-115">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="f9414-115">One of the following:</span></span> <ul><li><span data-ttu-id="f9414-116">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="f9414-116">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="f9414-117">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f9414-117">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="f9414-118">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="f9414-118">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="f9414-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9414-119">Properties</span></span>
| <span data-ttu-id="f9414-120">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="f9414-120">Property</span></span>  | <span data-ttu-id="f9414-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9414-121">Type</span></span>   | <span data-ttu-id="f9414-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9414-122">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="f9414-123">address</span><span class="sxs-lookup"><span data-stu-id="f9414-123">address</span></span> | [<span data-ttu-id="f9414-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f9414-124">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="f9414-125">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="f9414-125">The street address of the location.</span></span> |
| <span data-ttu-id="f9414-126">coordenadas</span><span class="sxs-lookup"><span data-stu-id="f9414-126">coordinates</span></span> | [<span data-ttu-id="f9414-127">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f9414-127">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="f9414-128">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="f9414-128">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="f9414-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f9414-129">displayName</span></span>  | <span data-ttu-id="f9414-130">String</span><span class="sxs-lookup"><span data-stu-id="f9414-130">String</span></span> | <span data-ttu-id="f9414-131">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="f9414-131">The name associated with the location.</span></span>                       |
| <span data-ttu-id="f9414-132">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f9414-132">locationEmailAddress</span></span> | <span data-ttu-id="f9414-133">String</span><span class="sxs-lookup"><span data-stu-id="f9414-133">String</span></span> | <span data-ttu-id="f9414-134">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="f9414-134">Optional email address of the location.</span></span> |
| <span data-ttu-id="f9414-135">locationUri</span><span class="sxs-lookup"><span data-stu-id="f9414-135">locationUri</span></span> | <span data-ttu-id="f9414-136">String</span><span class="sxs-lookup"><span data-stu-id="f9414-136">String</span></span> | <span data-ttu-id="f9414-137">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="f9414-137">Optional URI representing the location.</span></span> |
| <span data-ttu-id="f9414-138">locationType</span><span class="sxs-lookup"><span data-stu-id="f9414-138">locationType</span></span> | <span data-ttu-id="f9414-139">String</span><span class="sxs-lookup"><span data-stu-id="f9414-139">String</span></span> | <span data-ttu-id="f9414-140">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="f9414-140">The type of location.</span></span> <span data-ttu-id="f9414-141">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="f9414-141">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="f9414-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9414-142">Read-only.</span></span>|
| <span data-ttu-id="f9414-143">uniqueId</span><span class="sxs-lookup"><span data-stu-id="f9414-143">uniqueId</span></span> | <span data-ttu-id="f9414-144">String</span><span class="sxs-lookup"><span data-stu-id="f9414-144">String</span></span> | <span data-ttu-id="f9414-145">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="f9414-145">For internal use only.</span></span>|
| <span data-ttu-id="f9414-146">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="f9414-146">uniqueIdType</span></span> | <span data-ttu-id="f9414-147">String</span><span class="sxs-lookup"><span data-stu-id="f9414-147">String</span></span> | <span data-ttu-id="f9414-148">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="f9414-148">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f9414-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9414-149">JSON representation</span></span>

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
  "locationUri": "string",
  "locationType": "string",
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
