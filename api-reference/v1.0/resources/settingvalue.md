# <a name="settingvalue-resource-type"></a><span data-ttu-id="0d835-101">Tipo de recurso settingValue</span><span class="sxs-lookup"><span data-stu-id="0d835-101">settingValue resource type</span></span>

<span data-ttu-id="0d835-102">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="0d835-102">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="0d835-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d835-103">Properties</span></span>

| <span data-ttu-id="0d835-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d835-104">Property</span></span> | <span data-ttu-id="0d835-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d835-105">Type</span></span> | <span data-ttu-id="0d835-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d835-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0d835-107">name</span><span class="sxs-lookup"><span data-stu-id="0d835-107">name</span></span>|<span data-ttu-id="0d835-108">String</span><span class="sxs-lookup"><span data-stu-id="0d835-108">String</span></span>| <span data-ttu-id="0d835-109">Nome da configuração (como definido pelo [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="0d835-109">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="0d835-110">valor</span><span class="sxs-lookup"><span data-stu-id="0d835-110">value</span></span>|<span data-ttu-id="0d835-111">String</span><span class="sxs-lookup"><span data-stu-id="0d835-111">String</span></span>| <span data-ttu-id="0d835-112">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="0d835-112">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="0d835-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d835-113">JSON representation</span></span>

<span data-ttu-id="0d835-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d835-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->