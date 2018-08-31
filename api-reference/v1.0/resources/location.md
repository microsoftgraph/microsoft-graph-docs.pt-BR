# <a name="location-resource-type"></a><span data-ttu-id="0ba51-101">Tipo de recurso Location</span><span class="sxs-lookup"><span data-stu-id="0ba51-101">Location resource type</span></span>

<span data-ttu-id="0ba51-102">Representa informações de localização para um [evento](event.md).</span><span class="sxs-lookup"><span data-stu-id="0ba51-102">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="0ba51-103">Existem várias maneiras de criar eventos em um calendário, por exemplo, por meio de um aplicativo, usando a API REST [criar evento](../api/user_post_events.md), ou manualmente, usando a interface do usuário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="0ba51-103">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user_post_events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="0ba51-104">Quando você cria um evento usando a interface do usuário, é possível especificar o local como texto sem formatação (por exemplo, "Bar de Harry"), ou na lista de salas fornecida pelo Outlook, pela [Sugestão Automática do Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) ou pela [pesquisa local do Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="0ba51-104">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="0ba51-105">Dependendo de como um evento é criado, o Outlook pode definir a propriedade **locationType** somente leitura de maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="0ba51-105">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="0ba51-106">Como o evento foi criado</span><span class="sxs-lookup"><span data-stu-id="0ba51-106">How event was created</span></span>  | <span data-ttu-id="0ba51-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ba51-107">Property</span></span>   | <span data-ttu-id="0ba51-108">Valor esperado</span><span class="sxs-lookup"><span data-stu-id="0ba51-108">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="0ba51-109">API REST [criar evento](../api/user_post_events.md)</span><span class="sxs-lookup"><span data-stu-id="0ba51-109">[create event](../api/user_post_events.md) REST API</span></span> | <span data-ttu-id="0ba51-110">**locationType**</span><span class="sxs-lookup"><span data-stu-id="0ba51-110">**locationType**</span></span> | `default` |
| <span data-ttu-id="0ba51-111">Interface do usuário no Outlook</span><span class="sxs-lookup"><span data-stu-id="0ba51-111">User interface in Outlook</span></span> | <span data-ttu-id="0ba51-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="0ba51-112">**locationType**</span></span> | <span data-ttu-id="0ba51-113">Uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="0ba51-113">One of the following:</span></span> <ul><li><span data-ttu-id="0ba51-114">`default` para um local inserido como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="0ba51-114">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="0ba51-115">`conferenceRoom` para uma sala fornecida pela lista de salas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="0ba51-115">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="0ba51-116">Ou qualquer uma desta lista (`homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`) para um local da Sugestão Automática do Bing ou da pesquisa local do Bing.</span><span class="sxs-lookup"><span data-stu-id="0ba51-116">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="0ba51-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ba51-117">Properties</span></span>
| <span data-ttu-id="0ba51-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ba51-118">Property</span></span>  | <span data-ttu-id="0ba51-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ba51-119">Type</span></span>   | <span data-ttu-id="0ba51-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ba51-120">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="0ba51-121">address</span><span class="sxs-lookup"><span data-stu-id="0ba51-121">address</span></span> | [<span data-ttu-id="0ba51-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="0ba51-122">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="0ba51-123">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="0ba51-123">The street address of the location.</span></span> |
| <span data-ttu-id="0ba51-124">coordenadas</span><span class="sxs-lookup"><span data-stu-id="0ba51-124">coordinates</span></span> | [<span data-ttu-id="0ba51-125">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="0ba51-125">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="0ba51-126">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="0ba51-126">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="0ba51-127">displayName</span><span class="sxs-lookup"><span data-stu-id="0ba51-127">displayName</span></span>  | <span data-ttu-id="0ba51-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ba51-128">String</span></span> | <span data-ttu-id="0ba51-129">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="0ba51-129">The name associated with the location.</span></span>                       |
| <span data-ttu-id="0ba51-130">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0ba51-130">locationEmailAddress</span></span> | <span data-ttu-id="0ba51-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ba51-131">String</span></span> | <span data-ttu-id="0ba51-132">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="0ba51-132">Optional email address of the location.</span></span>              |
| <span data-ttu-id="0ba51-133">locationUri</span><span class="sxs-lookup"><span data-stu-id="0ba51-133">locationUri</span></span> | <span data-ttu-id="0ba51-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ba51-134">String</span></span> | <span data-ttu-id="0ba51-135">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="0ba51-135">Optional URI representing the location.</span></span> |
| <span data-ttu-id="0ba51-136">locationType</span><span class="sxs-lookup"><span data-stu-id="0ba51-136">locationType</span></span> | <span data-ttu-id="0ba51-137">locationType</span><span class="sxs-lookup"><span data-stu-id="0ba51-137">locationType</span></span> | <span data-ttu-id="0ba51-138">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="0ba51-138">The type of location.</span></span> <span data-ttu-id="0ba51-139">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="0ba51-139">The possible values are `default`, `conferenceRoom`, `homeAddress`, `businessAddress`, `geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`, , or .</span></span> <span data-ttu-id="0ba51-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ba51-140">Read-only.</span></span>|
| <span data-ttu-id="0ba51-141">uniqueId</span><span class="sxs-lookup"><span data-stu-id="0ba51-141">uniqueId</span></span> | <span data-ttu-id="0ba51-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ba51-142">String</span></span> | <span data-ttu-id="0ba51-143">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="0ba51-143">For internal use only.</span></span>|
| <span data-ttu-id="0ba51-144">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="0ba51-144">uniqueIdType</span></span> | <span data-ttu-id="0ba51-145">locationUniqueIdType</span><span class="sxs-lookup"><span data-stu-id="0ba51-145">locationUniqueIdType values</span></span> | <span data-ttu-id="0ba51-146">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="0ba51-146">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ba51-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ba51-147">JSON representation</span></span>

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
