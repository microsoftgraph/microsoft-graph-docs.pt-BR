# <a name="timestamp-resource-type"></a><span data-ttu-id="bfe6f-101">tipo de recurso timeStamp</span><span class="sxs-lookup"><span data-stu-id="bfe6f-101">timeStamp resource type</span></span>

<span data-ttu-id="bfe6f-102">Informações de data e hora para um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="bfe6f-102">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfe6f-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfe6f-103">JSON representation</span></span>

<span data-ttu-id="bfe6f-104">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bfe6f-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="bfe6f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfe6f-105">Properties</span></span>
| <span data-ttu-id="bfe6f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfe6f-106">Property</span></span>       | <span data-ttu-id="bfe6f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfe6f-107">Type</span></span>    |<span data-ttu-id="bfe6f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfe6f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfe6f-109">data</span><span class="sxs-lookup"><span data-stu-id="bfe6f-109">date</span></span>|<span data-ttu-id="bfe6f-110">Data</span><span class="sxs-lookup"><span data-stu-id="bfe6f-110">Date</span></span>|<span data-ttu-id="bfe6f-111">A parte da data do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="bfe6f-111">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="bfe6f-112">hora</span><span class="sxs-lookup"><span data-stu-id="bfe6f-112">time</span></span>|<span data-ttu-id="bfe6f-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bfe6f-113">TimeOfDay</span></span>|<span data-ttu-id="bfe6f-114">A parte da hora do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="bfe6f-114">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="bfe6f-115">timeZone</span><span class="sxs-lookup"><span data-stu-id="bfe6f-115">timeZone</span></span>|<span data-ttu-id="bfe6f-116">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfe6f-116">String</span></span>|<span data-ttu-id="bfe6f-117">A parte do fuso horário do carimbo de data/hora, que é uma das 24 áreas longitudinais no mundo.</span><span class="sxs-lookup"><span data-stu-id="bfe6f-117">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->