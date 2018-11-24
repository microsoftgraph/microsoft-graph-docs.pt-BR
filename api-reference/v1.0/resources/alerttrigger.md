# <a name="alerttrigger-resource-type"></a><span data-ttu-id="9b89f-101">tipo de recurso de alertTrigger</span><span class="sxs-lookup"><span data-stu-id="9b89f-101">alertTrigger resource type</span></span>

<span data-ttu-id="9b89f-102">Contém informações sobre as propriedades que disparou uma detecção (Propriedades existirem na entidade alerta).</span><span class="sxs-lookup"><span data-stu-id="9b89f-102">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="9b89f-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b89f-103">Properties</span></span>

| <span data-ttu-id="9b89f-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b89f-104">Property</span></span>   | <span data-ttu-id="9b89f-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b89f-105">Type</span></span>|<span data-ttu-id="9b89f-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b89f-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b89f-107">name</span><span class="sxs-lookup"><span data-stu-id="9b89f-107">name</span></span>|<span data-ttu-id="9b89f-108">String</span><span class="sxs-lookup"><span data-stu-id="9b89f-108">String</span></span>|<span data-ttu-id="9b89f-109">Nome da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="9b89f-109">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="9b89f-110">type</span><span class="sxs-lookup"><span data-stu-id="9b89f-110">type</span></span>|<span data-ttu-id="9b89f-111">String</span><span class="sxs-lookup"><span data-stu-id="9b89f-111">String</span></span>|<span data-ttu-id="9b89f-112">Tipo da propriedade no par de chave: valor de interpretação.</span><span class="sxs-lookup"><span data-stu-id="9b89f-112">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="9b89f-113">Por exemplo, String, Boolean, etc.</span><span class="sxs-lookup"><span data-stu-id="9b89f-113">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="9b89f-114">valor</span><span class="sxs-lookup"><span data-stu-id="9b89f-114">value</span></span>|<span data-ttu-id="9b89f-115">String</span><span class="sxs-lookup"><span data-stu-id="9b89f-115">String</span></span>|<span data-ttu-id="9b89f-116">Valor da propriedade servindo como um gatilho de detecção.</span><span class="sxs-lookup"><span data-stu-id="9b89f-116">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b89f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b89f-117">JSON representation</span></span>

<span data-ttu-id="9b89f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b89f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="9b89f-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b89f-119">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->