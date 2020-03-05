---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9b590d011570981fd926a5e12a8c89e6059b3b41
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522915"
---
# <a name="location-resource-type"></a><span data-ttu-id="9d80c-103">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="9d80c-103">Location resource type</span></span>

<span data-ttu-id="9d80c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9d80c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d80c-105">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="9d80c-105">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="9d80c-106">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="9d80c-106">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="9d80c-107">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="9d80c-107">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="9d80c-108">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="9d80c-108">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="9d80c-109">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="9d80c-109">How event was created</span></span>  | <span data-ttu-id="9d80c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d80c-110">Property</span></span>   | <span data-ttu-id="9d80c-111">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="9d80c-111">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="9d80c-112">API REST [criar evento](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="9d80c-112">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="9d80c-113">**locationType**</span><span class="sxs-lookup"><span data-stu-id="9d80c-113">**locationType**</span></span> | `default` |
| <span data-ttu-id="9d80c-114">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="9d80c-114">User interface in Outlook</span></span> | <span data-ttu-id="9d80c-115">**locationType**</span><span class="sxs-lookup"><span data-stu-id="9d80c-115">**locationType**</span></span> | <span data-ttu-id="9d80c-116">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="9d80c-116">One of the following:</span></span> <ul><li><span data-ttu-id="9d80c-117">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="9d80c-117">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="9d80c-118">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="9d80c-118">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="9d80c-119">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="9d80c-119">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="9d80c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d80c-120">Properties</span></span>
| <span data-ttu-id="9d80c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d80c-121">Property</span></span>  | <span data-ttu-id="9d80c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d80c-122">Type</span></span>   | <span data-ttu-id="9d80c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d80c-123">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="9d80c-124">address</span><span class="sxs-lookup"><span data-stu-id="9d80c-124">address</span></span> | [<span data-ttu-id="9d80c-125">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9d80c-125">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="9d80c-126">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="9d80c-126">The street address of the location.</span></span> |
| <span data-ttu-id="9d80c-127">coordenadas</span><span class="sxs-lookup"><span data-stu-id="9d80c-127">coordinates</span></span> | [<span data-ttu-id="9d80c-128">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="9d80c-128">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="9d80c-129">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="9d80c-129">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="9d80c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="9d80c-130">displayName</span></span>  | <span data-ttu-id="9d80c-131">String</span><span class="sxs-lookup"><span data-stu-id="9d80c-131">String</span></span> | <span data-ttu-id="9d80c-132">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="9d80c-132">The name associated with the location.</span></span>                       |
| <span data-ttu-id="9d80c-133">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9d80c-133">locationEmailAddress</span></span> | <span data-ttu-id="9d80c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d80c-134">String</span></span> | <span data-ttu-id="9d80c-135">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="9d80c-135">Optional email address of the location.</span></span> |
| <span data-ttu-id="9d80c-136">locationUri</span><span class="sxs-lookup"><span data-stu-id="9d80c-136">locationUri</span></span> | <span data-ttu-id="9d80c-137">String</span><span class="sxs-lookup"><span data-stu-id="9d80c-137">String</span></span> | <span data-ttu-id="9d80c-138">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="9d80c-138">Optional URI representing the location.</span></span> |
| <span data-ttu-id="9d80c-139">locationType</span><span class="sxs-lookup"><span data-stu-id="9d80c-139">locationType</span></span> | <span data-ttu-id="9d80c-140">locationType</span><span class="sxs-lookup"><span data-stu-id="9d80c-140">locationType</span></span> | <span data-ttu-id="9d80c-141">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="9d80c-141">The type of location.</span></span> <span data-ttu-id="9d80c-142">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="9d80c-142">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="9d80c-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d80c-143">Read-only.</span></span>|
| <span data-ttu-id="9d80c-144">uniqueId</span><span class="sxs-lookup"><span data-stu-id="9d80c-144">uniqueId</span></span> | <span data-ttu-id="9d80c-145">String</span><span class="sxs-lookup"><span data-stu-id="9d80c-145">String</span></span> | <span data-ttu-id="9d80c-146">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="9d80c-146">For internal use only.</span></span>|
| <span data-ttu-id="9d80c-147">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="9d80c-147">uniqueIdType</span></span> | <span data-ttu-id="9d80c-148">String</span><span class="sxs-lookup"><span data-stu-id="9d80c-148">String</span></span> | <span data-ttu-id="9d80c-149">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="9d80c-149">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9d80c-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d80c-150">JSON representation</span></span>

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
