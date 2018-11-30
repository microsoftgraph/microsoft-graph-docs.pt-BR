---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
ms.openlocfilehash: 149af193864c2a0ecab67ab2c722c9c3b46e9293
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004971"
---
# <a name="location-resource-type"></a><span data-ttu-id="18aab-103">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="18aab-103">Location resource type</span></span>

<span data-ttu-id="18aab-104">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="18aab-104">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="18aab-105">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="18aab-105">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="18aab-106">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="18aab-106">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="18aab-107">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="18aab-107">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="18aab-108">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="18aab-108">How event was created</span></span>  | <span data-ttu-id="18aab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18aab-109">Property</span></span>   | <span data-ttu-id="18aab-110">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="18aab-110">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="18aab-111">API REST [criar evento](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="18aab-111">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="18aab-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="18aab-112">**locationType**</span></span> | `default` |
| <span data-ttu-id="18aab-113">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="18aab-113">User interface in Outlook</span></span> | <span data-ttu-id="18aab-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="18aab-114">**locationType**</span></span> | <span data-ttu-id="18aab-115">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="18aab-115">One of the following:</span></span> <ul><li><span data-ttu-id="18aab-116">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="18aab-116">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="18aab-117">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="18aab-117">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="18aab-118">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="18aab-118">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="18aab-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18aab-119">Properties</span></span>
| <span data-ttu-id="18aab-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18aab-120">Property</span></span>  | <span data-ttu-id="18aab-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="18aab-121">Type</span></span>   | <span data-ttu-id="18aab-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="18aab-122">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="18aab-123">address</span><span class="sxs-lookup"><span data-stu-id="18aab-123">address</span></span> | [<span data-ttu-id="18aab-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="18aab-124">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="18aab-125">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="18aab-125">The street address of the location.</span></span> |
| <span data-ttu-id="18aab-126">coordenadas</span><span class="sxs-lookup"><span data-stu-id="18aab-126">coordinates</span></span> | [<span data-ttu-id="18aab-127">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="18aab-127">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="18aab-128">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="18aab-128">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="18aab-129">displayName</span><span class="sxs-lookup"><span data-stu-id="18aab-129">displayName</span></span>  | <span data-ttu-id="18aab-130">String</span><span class="sxs-lookup"><span data-stu-id="18aab-130">String</span></span> | <span data-ttu-id="18aab-131">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="18aab-131">The name associated with the location.</span></span>                       |
| <span data-ttu-id="18aab-132">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="18aab-132">locationEmailAddress</span></span> | <span data-ttu-id="18aab-133">String</span><span class="sxs-lookup"><span data-stu-id="18aab-133">String</span></span> | <span data-ttu-id="18aab-134">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="18aab-134">Optional email address of the location.</span></span>              |
| <span data-ttu-id="18aab-135">locationUri</span><span class="sxs-lookup"><span data-stu-id="18aab-135">locationUri</span></span> | <span data-ttu-id="18aab-136">String</span><span class="sxs-lookup"><span data-stu-id="18aab-136">String</span></span> | <span data-ttu-id="18aab-137">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="18aab-137">Optional URI representing the location.</span></span> |
| <span data-ttu-id="18aab-138">locationType</span><span class="sxs-lookup"><span data-stu-id="18aab-138">locationType</span></span> | <span data-ttu-id="18aab-139">locationType</span><span class="sxs-lookup"><span data-stu-id="18aab-139">locationType</span></span> | <span data-ttu-id="18aab-140">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="18aab-140">The type of location.</span></span> <span data-ttu-id="18aab-141">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="18aab-141">The possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="18aab-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18aab-142">Read-only.</span></span>|
| <span data-ttu-id="18aab-143">uniqueId</span><span class="sxs-lookup"><span data-stu-id="18aab-143">uniqueId</span></span> | <span data-ttu-id="18aab-144">String</span><span class="sxs-lookup"><span data-stu-id="18aab-144">String</span></span> | <span data-ttu-id="18aab-145">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="18aab-145">For internal use only.</span></span>|
| <span data-ttu-id="18aab-146">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="18aab-146">uniqueIdType</span></span> | <span data-ttu-id="18aab-147">locationUniqueIdType</span><span class="sxs-lookup"><span data-stu-id="18aab-147">locationUniqueIdType</span></span> | <span data-ttu-id="18aab-148">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="18aab-148">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18aab-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18aab-149">JSON representation</span></span>

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
