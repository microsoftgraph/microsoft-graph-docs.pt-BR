# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="d868e-101">Tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="d868e-101">settingTemplateValue resource type</span></span>

<span data-ttu-id="d868e-102">Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="d868e-102">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="d868e-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d868e-103">Properties</span></span>

| <span data-ttu-id="d868e-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d868e-104">Property</span></span> | <span data-ttu-id="d868e-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="d868e-105">Type</span></span> | <span data-ttu-id="d868e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d868e-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d868e-107">defaultValue</span><span class="sxs-lookup"><span data-stu-id="d868e-107">DefaultValue</span></span>|<span data-ttu-id="d868e-108">String</span><span class="sxs-lookup"><span data-stu-id="d868e-108">String</span></span>| <span data-ttu-id="d868e-109">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="d868e-109">Default value for the setting.</span></span> |
|<span data-ttu-id="d868e-110">description</span><span class="sxs-lookup"><span data-stu-id="d868e-110">description</span></span>|<span data-ttu-id="d868e-111">String</span><span class="sxs-lookup"><span data-stu-id="d868e-111">String</span></span>| <span data-ttu-id="d868e-112">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="d868e-112">Description of the component.</span></span> |
|<span data-ttu-id="d868e-113">nome</span><span class="sxs-lookup"><span data-stu-id="d868e-113">name</span></span>|<span data-ttu-id="d868e-114">String</span><span class="sxs-lookup"><span data-stu-id="d868e-114">String</span></span>| <span data-ttu-id="d868e-115">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="d868e-115">Name of the setting.</span></span> |
|<span data-ttu-id="d868e-116">type</span><span class="sxs-lookup"><span data-stu-id="d868e-116">type</span></span>|<span data-ttu-id="d868e-117">String</span><span class="sxs-lookup"><span data-stu-id="d868e-117">String</span></span>| <span data-ttu-id="d868e-118">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="d868e-118">Key of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="d868e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d868e-119">JSON representation</span></span>

<span data-ttu-id="d868e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d868e-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->