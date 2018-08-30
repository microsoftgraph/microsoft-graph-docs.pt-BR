# <a name="responsestatus-resource-type"></a><span data-ttu-id="70a4b-101">Tipo de recurso responseStatus</span><span class="sxs-lookup"><span data-stu-id="70a4b-101">responseStatus resource type</span></span>

<span data-ttu-id="70a4b-102">O status de resposta de uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="70a4b-102">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="70a4b-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70a4b-103">Properties</span></span>

| <span data-ttu-id="70a4b-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70a4b-104">Property</span></span> | <span data-ttu-id="70a4b-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="70a4b-105">Type</span></span>           | <span data-ttu-id="70a4b-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a4b-106">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="70a4b-107">response</span><span class="sxs-lookup"><span data-stu-id="70a4b-107">response</span></span> | <span data-ttu-id="70a4b-108">ResponseType</span><span class="sxs-lookup"><span data-stu-id="70a4b-108">ResponseType</span></span>   | <span data-ttu-id="70a4b-109">O tipo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70a4b-109">The response type.</span></span> <span data-ttu-id="70a4b-110">Os valores possíveis são: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="70a4b-110">The possible values are `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`, , , , , , or .</span></span>
| <span data-ttu-id="70a4b-111">time</span><span class="sxs-lookup"><span data-stu-id="70a4b-111">time</span></span>     | <span data-ttu-id="70a4b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70a4b-112">DateTimeOffset</span></span> | <span data-ttu-id="70a4b-p102">A data e hora em que a resposta retornou. Usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="70a4b-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="70a4b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70a4b-116">JSON representation</span></span>

<span data-ttu-id="70a4b-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="70a4b-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
