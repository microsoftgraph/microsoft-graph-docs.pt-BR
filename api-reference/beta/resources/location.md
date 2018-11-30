---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
ms.openlocfilehash: fec075d37bfb2d7eca80f5007db53801dda96ed8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033234"
---
# <a name="location-resource-type"></a><span data-ttu-id="01bc7-103">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="01bc7-103">Location resource type</span></span>

> <span data-ttu-id="01bc7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="01bc7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01bc7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01bc7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01bc7-106">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="01bc7-106">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="01bc7-107">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="01bc7-107">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="01bc7-108">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="01bc7-108">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="01bc7-109">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="01bc7-109">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="01bc7-110">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="01bc7-110">How event was created</span></span>  | <span data-ttu-id="01bc7-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01bc7-111">Property</span></span>   | <span data-ttu-id="01bc7-112">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="01bc7-112">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="01bc7-113">API REST [criar evento](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="01bc7-113">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="01bc7-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="01bc7-114">**locationType**</span></span> | `default` |
| <span data-ttu-id="01bc7-115">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="01bc7-115">User interface in Outlook</span></span> | <span data-ttu-id="01bc7-116">**locationType**</span><span class="sxs-lookup"><span data-stu-id="01bc7-116">**locationType**</span></span> | <span data-ttu-id="01bc7-117">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="01bc7-117">One of the following:</span></span> <ul><li><span data-ttu-id="01bc7-118">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="01bc7-118">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="01bc7-119">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="01bc7-119">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="01bc7-120">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="01bc7-120">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="01bc7-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01bc7-121">Properties</span></span>
| <span data-ttu-id="01bc7-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01bc7-122">Property</span></span>  | <span data-ttu-id="01bc7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="01bc7-123">Type</span></span>   | <span data-ttu-id="01bc7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="01bc7-124">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="01bc7-125">address</span><span class="sxs-lookup"><span data-stu-id="01bc7-125">address</span></span> | [<span data-ttu-id="01bc7-126">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="01bc7-126">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="01bc7-127">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="01bc7-127">The street address of the location.</span></span> |
| <span data-ttu-id="01bc7-128">coordenadas</span><span class="sxs-lookup"><span data-stu-id="01bc7-128">coordinates</span></span> | [<span data-ttu-id="01bc7-129">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="01bc7-129">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="01bc7-130">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="01bc7-130">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="01bc7-131">displayName</span><span class="sxs-lookup"><span data-stu-id="01bc7-131">displayName</span></span>  | <span data-ttu-id="01bc7-132">String</span><span class="sxs-lookup"><span data-stu-id="01bc7-132">String</span></span> | <span data-ttu-id="01bc7-133">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="01bc7-133">The name associated with the location.</span></span>                       |
| <span data-ttu-id="01bc7-134">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="01bc7-134">locationEmailAddress</span></span> | <span data-ttu-id="01bc7-135">String</span><span class="sxs-lookup"><span data-stu-id="01bc7-135">String</span></span> | <span data-ttu-id="01bc7-136">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="01bc7-136">Optional email address of the location.</span></span> |
| <span data-ttu-id="01bc7-137">locationUri</span><span class="sxs-lookup"><span data-stu-id="01bc7-137">locationUri</span></span> | <span data-ttu-id="01bc7-138">String</span><span class="sxs-lookup"><span data-stu-id="01bc7-138">String</span></span> | <span data-ttu-id="01bc7-139">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="01bc7-139">Optional URI representing the location.</span></span> |
| <span data-ttu-id="01bc7-140">locationType</span><span class="sxs-lookup"><span data-stu-id="01bc7-140">locationType</span></span> | <span data-ttu-id="01bc7-141">String</span><span class="sxs-lookup"><span data-stu-id="01bc7-141">String</span></span> | <span data-ttu-id="01bc7-142">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="01bc7-142">The type of location.</span></span> <span data-ttu-id="01bc7-143">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="01bc7-143">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="01bc7-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01bc7-144">Read-only.</span></span>|
| <span data-ttu-id="01bc7-145">uniqueId</span><span class="sxs-lookup"><span data-stu-id="01bc7-145">uniqueId</span></span> | <span data-ttu-id="01bc7-146">String</span><span class="sxs-lookup"><span data-stu-id="01bc7-146">String</span></span> | <span data-ttu-id="01bc7-147">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="01bc7-147">For internal use only.</span></span>|
| <span data-ttu-id="01bc7-148">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="01bc7-148">uniqueIdType</span></span> | <span data-ttu-id="01bc7-149">String</span><span class="sxs-lookup"><span data-stu-id="01bc7-149">String</span></span> | <span data-ttu-id="01bc7-150">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="01bc7-150">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="01bc7-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01bc7-151">JSON representation</span></span>

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
