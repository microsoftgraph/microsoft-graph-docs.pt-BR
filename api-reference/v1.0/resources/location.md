---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3f1839bdb7bb06dc0df11020ef14e51cf53d2d5e
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43441478"
---
# <a name="location-resource-type"></a><span data-ttu-id="0b6ae-103">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="0b6ae-103">Location resource type</span></span>

<span data-ttu-id="0b6ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b6ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b6ae-105">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="0b6ae-105">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="0b6ae-106">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-106">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="0b6ae-107">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="0b6ae-107">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="0b6ae-108">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-108">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="0b6ae-109">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="0b6ae-109">How event was created</span></span>  | <span data-ttu-id="0b6ae-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b6ae-110">Property</span></span>   | <span data-ttu-id="0b6ae-111">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="0b6ae-111">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="0b6ae-112">API REST [criar evento](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="0b6ae-112">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="0b6ae-113">**locationType**</span><span class="sxs-lookup"><span data-stu-id="0b6ae-113">**locationType**</span></span> | `default` |
| <span data-ttu-id="0b6ae-114">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="0b6ae-114">User interface in Outlook</span></span> | <span data-ttu-id="0b6ae-115">**locationType**</span><span class="sxs-lookup"><span data-stu-id="0b6ae-115">**locationType**</span></span> | <span data-ttu-id="0b6ae-116">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="0b6ae-116">One of the following:</span></span> <ul><li><span data-ttu-id="0b6ae-117">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-117">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="0b6ae-118">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-118">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="0b6ae-119">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-119">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="0b6ae-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b6ae-120">Properties</span></span>
| <span data-ttu-id="0b6ae-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b6ae-121">Property</span></span>  | <span data-ttu-id="0b6ae-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b6ae-122">Type</span></span>   | <span data-ttu-id="0b6ae-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b6ae-123">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="0b6ae-124">address</span><span class="sxs-lookup"><span data-stu-id="0b6ae-124">address</span></span> | [<span data-ttu-id="0b6ae-125">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="0b6ae-125">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="0b6ae-126">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-126">The street address of the location.</span></span> |
| <span data-ttu-id="0b6ae-127">coordenadas</span><span class="sxs-lookup"><span data-stu-id="0b6ae-127">coordinates</span></span> | [<span data-ttu-id="0b6ae-128">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="0b6ae-128">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="0b6ae-129">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-129">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="0b6ae-130">displayName</span><span class="sxs-lookup"><span data-stu-id="0b6ae-130">displayName</span></span>  | <span data-ttu-id="0b6ae-131">String</span><span class="sxs-lookup"><span data-stu-id="0b6ae-131">String</span></span> | <span data-ttu-id="0b6ae-132">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-132">The name associated with the location.</span></span>                       |
| <span data-ttu-id="0b6ae-133">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0b6ae-133">locationEmailAddress</span></span> | <span data-ttu-id="0b6ae-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b6ae-134">String</span></span> | <span data-ttu-id="0b6ae-135">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-135">Optional email address of the location.</span></span>              |
| <span data-ttu-id="0b6ae-136">locationUri</span><span class="sxs-lookup"><span data-stu-id="0b6ae-136">locationUri</span></span> | <span data-ttu-id="0b6ae-137">String</span><span class="sxs-lookup"><span data-stu-id="0b6ae-137">String</span></span> | <span data-ttu-id="0b6ae-138">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-138">Optional URI representing the location.</span></span> |
| <span data-ttu-id="0b6ae-139">locationType</span><span class="sxs-lookup"><span data-stu-id="0b6ae-139">locationType</span></span> | <span data-ttu-id="0b6ae-140">locationType</span><span class="sxs-lookup"><span data-stu-id="0b6ae-140">locationType</span></span> | <span data-ttu-id="0b6ae-141">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-141">The type of location.</span></span> <span data-ttu-id="0b6ae-142">Os valores possíveis são: `default` , `conferenceRoom` , `homeAddress` , `businessAddress` , `geoCoordinates` , `streetAddress` , `hotel` , `restaurant` , `localBusiness` , `postalAddress` .</span><span class="sxs-lookup"><span data-stu-id="0b6ae-142">The possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="0b6ae-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-143">Read-only.</span></span>|
| <span data-ttu-id="0b6ae-144">uniqueId</span><span class="sxs-lookup"><span data-stu-id="0b6ae-144">uniqueId</span></span> | <span data-ttu-id="0b6ae-145">String</span><span class="sxs-lookup"><span data-stu-id="0b6ae-145">String</span></span> | <span data-ttu-id="0b6ae-146">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-146">For internal use only.</span></span>|
| <span data-ttu-id="0b6ae-147">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="0b6ae-147">uniqueIdType</span></span> | <span data-ttu-id="0b6ae-148">locationUniqueIdType</span><span class="sxs-lookup"><span data-stu-id="0b6ae-148">locationUniqueIdType</span></span> | <span data-ttu-id="0b6ae-149">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="0b6ae-149">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0b6ae-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b6ae-150">JSON representation</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
