# <a name="alerttrigger-resource-type"></a><span data-ttu-id="86e82-101">Tipo de recurso alertTrigger</span><span class="sxs-lookup"><span data-stu-id="86e82-101">alertTrigger resource type</span></span>

<span data-ttu-id="86e82-102">Contém informações sobre as propriedades que dispararam uma detecção (as propriedades existem na entidade alerta).</span><span class="sxs-lookup"><span data-stu-id="86e82-102">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="86e82-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86e82-103">Properties</span></span>

| <span data-ttu-id="86e82-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86e82-104">Property</span></span>   | <span data-ttu-id="86e82-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="86e82-105">Type</span></span>|<span data-ttu-id="86e82-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="86e82-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86e82-107">name</span><span class="sxs-lookup"><span data-stu-id="86e82-107">name</span></span>|<span data-ttu-id="86e82-108">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="86e82-108">String</span></span>|<span data-ttu-id="86e82-109">Nome da propriedade servindo como um disparo de detecção.</span><span class="sxs-lookup"><span data-stu-id="86e82-109">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="86e82-110">type</span><span class="sxs-lookup"><span data-stu-id="86e82-110">type</span></span>|<span data-ttu-id="86e82-111">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="86e82-111">String</span></span>|<span data-ttu-id="86e82-112">Tipo da propriedade no par de chave:valor para interpretação.</span><span class="sxs-lookup"><span data-stu-id="86e82-112">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="86e82-113">Por exemplo, sequência de caracteres, Booleano, etc.</span><span class="sxs-lookup"><span data-stu-id="86e82-113">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="86e82-114">value</span><span class="sxs-lookup"><span data-stu-id="86e82-114">value</span></span>|<span data-ttu-id="86e82-115">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="86e82-115">String</span></span>|<span data-ttu-id="86e82-116">Nome da propriedade que serve como um disparo de detecção.</span><span class="sxs-lookup"><span data-stu-id="86e82-116">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86e82-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86e82-117">JSON representation</span></span>

<span data-ttu-id="86e82-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86e82-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="86e82-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86e82-119">Example</span></span>

```json
{
  "name": "endpointAddress",
  "type": "networkConnection.sourceAddress",
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