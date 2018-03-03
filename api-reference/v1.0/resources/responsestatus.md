# <a name="responsestatus-resource-type"></a><span data-ttu-id="7e429-101">Tipo de recurso responseStatus</span><span class="sxs-lookup"><span data-stu-id="7e429-101">responseStatus resource type</span></span>

<span data-ttu-id="7e429-102">O status de resposta de uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="7e429-102">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="7e429-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e429-103">Properties</span></span>

| <span data-ttu-id="7e429-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e429-104">Property</span></span> | <span data-ttu-id="7e429-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e429-105">Type</span></span>           | <span data-ttu-id="7e429-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e429-106">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="7e429-107">response</span><span class="sxs-lookup"><span data-stu-id="7e429-107">response</span></span> | <span data-ttu-id="7e429-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e429-108">String</span></span>         | <span data-ttu-id="7e429-109">O tipo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e429-109">The response type.</span></span> <span data-ttu-id="7e429-110">Os valores possíveis são: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="7e429-110">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="7e429-111">time</span><span class="sxs-lookup"><span data-stu-id="7e429-111">time</span></span>     | <span data-ttu-id="7e429-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e429-112">DateTimeOffset</span></span> | <span data-ttu-id="7e429-113">A data e hora em que a resposta retornou.</span><span class="sxs-lookup"><span data-stu-id="7e429-113">The date and time that the response was returned.</span></span> <span data-ttu-id="7e429-114">Usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7e429-114">It uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7e429-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7e429-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'` Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e429-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e429-116">JSON representation</span></span>

<span data-ttu-id="7e429-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7e429-117">Here is a JSON representation of the resource</span></span>

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
