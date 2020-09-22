---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
localization_priority: Normal
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 764dcfd92095a2432cd42527ba98af1ed0e5c535
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073576"
---
# <a name="location-resource-type"></a><span data-ttu-id="17c3b-103">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="17c3b-103">Location resource type</span></span>

<span data-ttu-id="17c3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17c3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17c3b-105">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="17c3b-105">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="17c3b-106">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="17c3b-106">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="17c3b-107">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="17c3b-107">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="17c3b-108">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="17c3b-108">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="17c3b-109">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="17c3b-109">How event was created</span></span>  | <span data-ttu-id="17c3b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17c3b-110">Property</span></span>   | <span data-ttu-id="17c3b-111">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="17c3b-111">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="17c3b-112">API REST [criar evento](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="17c3b-112">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="17c3b-113">**locationType**</span><span class="sxs-lookup"><span data-stu-id="17c3b-113">**locationType**</span></span> | `default` |
| <span data-ttu-id="17c3b-114">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="17c3b-114">User interface in Outlook</span></span> | <span data-ttu-id="17c3b-115">**locationType**</span><span class="sxs-lookup"><span data-stu-id="17c3b-115">**locationType**</span></span> | <span data-ttu-id="17c3b-116">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="17c3b-116">One of the following:</span></span> <ul><li><span data-ttu-id="17c3b-117">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="17c3b-117">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="17c3b-118">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="17c3b-118">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="17c3b-119">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="17c3b-119">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="17c3b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17c3b-120">Properties</span></span>
| <span data-ttu-id="17c3b-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17c3b-121">Property</span></span>  | <span data-ttu-id="17c3b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="17c3b-122">Type</span></span>   | <span data-ttu-id="17c3b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="17c3b-123">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="17c3b-124">address</span><span class="sxs-lookup"><span data-stu-id="17c3b-124">address</span></span> | [<span data-ttu-id="17c3b-125">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="17c3b-125">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="17c3b-126">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="17c3b-126">The street address of the location.</span></span> |
| <span data-ttu-id="17c3b-127">coordenadas</span><span class="sxs-lookup"><span data-stu-id="17c3b-127">coordinates</span></span> | [<span data-ttu-id="17c3b-128">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="17c3b-128">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="17c3b-129">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="17c3b-129">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="17c3b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="17c3b-130">displayName</span></span>  | <span data-ttu-id="17c3b-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c3b-131">String</span></span> | <span data-ttu-id="17c3b-132">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="17c3b-132">The name associated with the location.</span></span>                       |
| <span data-ttu-id="17c3b-133">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="17c3b-133">locationEmailAddress</span></span> | <span data-ttu-id="17c3b-134">String</span><span class="sxs-lookup"><span data-stu-id="17c3b-134">String</span></span> | <span data-ttu-id="17c3b-135">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="17c3b-135">Optional email address of the location.</span></span> |
| <span data-ttu-id="17c3b-136">locationUri</span><span class="sxs-lookup"><span data-stu-id="17c3b-136">locationUri</span></span> | <span data-ttu-id="17c3b-137">String</span><span class="sxs-lookup"><span data-stu-id="17c3b-137">String</span></span> | <span data-ttu-id="17c3b-138">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="17c3b-138">Optional URI representing the location.</span></span> |
| <span data-ttu-id="17c3b-139">locationType</span><span class="sxs-lookup"><span data-stu-id="17c3b-139">locationType</span></span> | <span data-ttu-id="17c3b-140">locationType</span><span class="sxs-lookup"><span data-stu-id="17c3b-140">locationType</span></span> | <span data-ttu-id="17c3b-141">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="17c3b-141">The type of location.</span></span> <span data-ttu-id="17c3b-142">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="17c3b-142">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="17c3b-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17c3b-143">Read-only.</span></span>|
| <span data-ttu-id="17c3b-144">uniqueId</span><span class="sxs-lookup"><span data-stu-id="17c3b-144">uniqueId</span></span> | <span data-ttu-id="17c3b-145">String</span><span class="sxs-lookup"><span data-stu-id="17c3b-145">String</span></span> | <span data-ttu-id="17c3b-146">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="17c3b-146">For internal use only.</span></span>|
| <span data-ttu-id="17c3b-147">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="17c3b-147">uniqueIdType</span></span> | <span data-ttu-id="17c3b-148">String</span><span class="sxs-lookup"><span data-stu-id="17c3b-148">String</span></span> | <span data-ttu-id="17c3b-149">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="17c3b-149">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="17c3b-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17c3b-150">JSON representation</span></span>

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
  "suppressions": []
}
-->


