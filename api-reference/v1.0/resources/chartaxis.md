# <a name="chartaxis-resource-type"></a><span data-ttu-id="2e6af-101">Tipo de recurso ChartAxis</span><span class="sxs-lookup"><span data-stu-id="2e6af-101">ChartAxis resource type</span></span>

<span data-ttu-id="2e6af-102">Representa um único eixo em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="2e6af-102">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="2e6af-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e6af-103">Methods</span></span>

| <span data-ttu-id="2e6af-104">Método</span><span class="sxs-lookup"><span data-stu-id="2e6af-104">Method</span></span>           | <span data-ttu-id="2e6af-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e6af-105">Return Type</span></span>    |<span data-ttu-id="2e6af-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e6af-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e6af-107">Obter ChartAxis</span><span class="sxs-lookup"><span data-stu-id="2e6af-107">Get ChartAxis</span></span>](../api/chartaxis_get.md) | [<span data-ttu-id="2e6af-108">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="2e6af-108">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="2e6af-109">Propriedades de leitura e relacionamentos do objeto chartAxis.</span><span class="sxs-lookup"><span data-stu-id="2e6af-109">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="2e6af-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2e6af-110">Update</span></span>](../api/chartaxis_update.md) | [<span data-ttu-id="2e6af-111">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="2e6af-111">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="2e6af-112">Atualizar o objeto ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="2e6af-112">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2e6af-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e6af-113">Properties</span></span>
| <span data-ttu-id="2e6af-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e6af-114">Property</span></span>     | <span data-ttu-id="2e6af-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e6af-115">Type</span></span>   |<span data-ttu-id="2e6af-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e6af-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2e6af-117">id</span><span class="sxs-lookup"><span data-stu-id="2e6af-117">id</span></span>       |<span data-ttu-id="2e6af-118">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e6af-118">string</span></span>   | <span data-ttu-id="2e6af-119">Identificador único.</span><span class="sxs-lookup"><span data-stu-id="2e6af-119">Unique Identifier</span></span> <span data-ttu-id="2e6af-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6af-120">Read-only.</span></span>|
|<span data-ttu-id="2e6af-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="2e6af-121">majorUnit</span></span>|<span data-ttu-id="2e6af-122">Json</span><span class="sxs-lookup"><span data-stu-id="2e6af-122">Json</span></span>|<span data-ttu-id="2e6af-p102">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="2e6af-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="2e6af-126">maximum</span><span class="sxs-lookup"><span data-stu-id="2e6af-126">maximum</span></span>|<span data-ttu-id="2e6af-127">Json</span><span class="sxs-lookup"><span data-stu-id="2e6af-127">Json</span></span>|<span data-ttu-id="2e6af-p103">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="2e6af-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="2e6af-131">minimum</span><span class="sxs-lookup"><span data-stu-id="2e6af-131">minimum</span></span>|<span data-ttu-id="2e6af-132">Json</span><span class="sxs-lookup"><span data-stu-id="2e6af-132">Json</span></span>|<span data-ttu-id="2e6af-p104">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="2e6af-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="2e6af-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="2e6af-136">minorUnit</span></span>|<span data-ttu-id="2e6af-137">Json</span><span class="sxs-lookup"><span data-stu-id="2e6af-137">Json</span></span>|<span data-ttu-id="2e6af-p105">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="2e6af-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e6af-141">Relações</span><span class="sxs-lookup"><span data-stu-id="2e6af-141">Relationships</span></span>
| <span data-ttu-id="2e6af-142">Relação</span><span class="sxs-lookup"><span data-stu-id="2e6af-142">Relationship</span></span> | <span data-ttu-id="2e6af-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e6af-143">Type</span></span>   |<span data-ttu-id="2e6af-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e6af-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e6af-145">formato</span><span class="sxs-lookup"><span data-stu-id="2e6af-145">format</span></span>|[<span data-ttu-id="2e6af-146">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="2e6af-146">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="2e6af-p106">Representa a formatação de um objeto chart, que inclui formatação de linha e de fonte. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6af-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="2e6af-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="2e6af-149">majorGridlines</span></span>|[<span data-ttu-id="2e6af-150">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="2e6af-150">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="2e6af-p107">Retorna um objeto gridlines que representa as principais linhas de grade do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6af-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="2e6af-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="2e6af-153">minorGridlines</span></span>|[<span data-ttu-id="2e6af-154">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="2e6af-154">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="2e6af-p108">Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6af-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="2e6af-157">título</span><span class="sxs-lookup"><span data-stu-id="2e6af-157">title</span></span>|[<span data-ttu-id="2e6af-158">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="2e6af-158">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="2e6af-p109">Representa o título do eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e6af-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e6af-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e6af-161">JSON representation</span></span>

<span data-ttu-id="2e6af-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e6af-162">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->