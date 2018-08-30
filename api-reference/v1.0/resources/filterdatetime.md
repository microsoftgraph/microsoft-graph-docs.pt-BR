# <a name="filterdatetime-resource-type"></a><span data-ttu-id="053a6-101">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="053a6-101">FilterDatetime resource type</span></span>

<span data-ttu-id="053a6-102">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="053a6-102">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="053a6-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="053a6-103">Properties</span></span>
| <span data-ttu-id="053a6-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="053a6-104">Property</span></span>     | <span data-ttu-id="053a6-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="053a6-105">Type</span></span>   |<span data-ttu-id="053a6-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="053a6-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="053a6-107">data</span><span class="sxs-lookup"><span data-stu-id="053a6-107">date</span></span>|<span data-ttu-id="053a6-108">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="053a6-108">string</span></span>|<span data-ttu-id="053a6-109">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="053a6-109">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="053a6-110">especificidade</span><span class="sxs-lookup"><span data-stu-id="053a6-110">specificity</span></span>|<span data-ttu-id="053a6-111">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="053a6-111">string</span></span>|<span data-ttu-id="053a6-112">Quão específica a data deve ser para manter os dados.</span><span class="sxs-lookup"><span data-stu-id="053a6-112">How specific the date should be used to keep data.</span></span> <span data-ttu-id="053a6-113">Por exemplo, se a data é 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtro manterá todas as linhas com uma data no mês de abril de 2009.</span><span class="sxs-lookup"><span data-stu-id="053a6-113">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: , , , , , .</span></span> <span data-ttu-id="053a6-114">Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="053a6-114">The possible values are `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="053a6-115">Relações</span><span class="sxs-lookup"><span data-stu-id="053a6-115">Relationships</span></span>
<span data-ttu-id="053a6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="053a6-116">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="053a6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="053a6-117">JSON representation</span></span>

<span data-ttu-id="053a6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="053a6-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->