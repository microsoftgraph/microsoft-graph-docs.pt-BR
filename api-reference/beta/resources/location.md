---
title: Tipo de recurso Location
description: Representa informações de localização para um evento.
localization_priority: Normal
ms.openlocfilehash: 650876596e2cf9336054957cfd4c95bf4dad16b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879398"
---
# <a name="location-resource-type"></a><span data-ttu-id="a7cb9-103">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="a7cb9-103">Location resource type</span></span>

> <span data-ttu-id="a7cb9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7cb9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7cb9-106">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="a7cb9-106">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="a7cb9-107">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user-post-events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-107">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="a7cb9-108">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="a7cb9-108">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="a7cb9-109">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-109">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="a7cb9-110">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="a7cb9-110">How event was created</span></span>  | <span data-ttu-id="a7cb9-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7cb9-111">Property</span></span>   | <span data-ttu-id="a7cb9-112">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="a7cb9-112">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="a7cb9-113">API REST [criar evento](../api/user-post-events.md)</span><span class="sxs-lookup"><span data-stu-id="a7cb9-113">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="a7cb9-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="a7cb9-114">**locationType**</span></span> | `default` |
| <span data-ttu-id="a7cb9-115">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="a7cb9-115">User interface in Outlook</span></span> | <span data-ttu-id="a7cb9-116">**locationType**</span><span class="sxs-lookup"><span data-stu-id="a7cb9-116">**locationType**</span></span> | <span data-ttu-id="a7cb9-117">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="a7cb9-117">One of the following:</span></span> <ul><li><span data-ttu-id="a7cb9-118">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-118">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="a7cb9-119">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-119">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="a7cb9-120">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-120">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="a7cb9-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7cb9-121">Properties</span></span>
| <span data-ttu-id="a7cb9-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7cb9-122">Property</span></span>  | <span data-ttu-id="a7cb9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7cb9-123">Type</span></span>   | <span data-ttu-id="a7cb9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7cb9-124">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="a7cb9-125">address</span><span class="sxs-lookup"><span data-stu-id="a7cb9-125">address</span></span> | [<span data-ttu-id="a7cb9-126">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a7cb9-126">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="a7cb9-127">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-127">The street address of the location.</span></span> |
| <span data-ttu-id="a7cb9-128">coordenadas</span><span class="sxs-lookup"><span data-stu-id="a7cb9-128">coordinates</span></span> | [<span data-ttu-id="a7cb9-129">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a7cb9-129">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="a7cb9-130">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-130">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="a7cb9-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a7cb9-131">displayName</span></span>  | <span data-ttu-id="a7cb9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7cb9-132">String</span></span> | <span data-ttu-id="a7cb9-133">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-133">The name associated with the location.</span></span>                       |
| <span data-ttu-id="a7cb9-134">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a7cb9-134">locationEmailAddress</span></span> | <span data-ttu-id="a7cb9-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7cb9-135">String</span></span> | <span data-ttu-id="a7cb9-136">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-136">Optional email address of the location.</span></span> |
| <span data-ttu-id="a7cb9-137">locationUri</span><span class="sxs-lookup"><span data-stu-id="a7cb9-137">locationUri</span></span> | <span data-ttu-id="a7cb9-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7cb9-138">String</span></span> | <span data-ttu-id="a7cb9-139">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-139">Optional URI representing the location.</span></span> |
| <span data-ttu-id="a7cb9-140">locationType</span><span class="sxs-lookup"><span data-stu-id="a7cb9-140">locationType</span></span> | <span data-ttu-id="a7cb9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7cb9-141">String</span></span> | <span data-ttu-id="a7cb9-142">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-142">The type of location.</span></span> <span data-ttu-id="a7cb9-143">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-143">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="a7cb9-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-144">Read-only.</span></span>|
| <span data-ttu-id="a7cb9-145">uniqueId</span><span class="sxs-lookup"><span data-stu-id="a7cb9-145">uniqueId</span></span> | <span data-ttu-id="a7cb9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7cb9-146">String</span></span> | <span data-ttu-id="a7cb9-147">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-147">For internal use only.</span></span>|
| <span data-ttu-id="a7cb9-148">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="a7cb9-148">uniqueIdType</span></span> | <span data-ttu-id="a7cb9-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7cb9-149">String</span></span> | <span data-ttu-id="a7cb9-150">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="a7cb9-150">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a7cb9-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7cb9-151">JSON representation</span></span>

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
