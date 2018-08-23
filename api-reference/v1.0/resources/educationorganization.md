# <a name="educationorganization-resource-type"></a><span data-ttu-id="71905-101">tipo de recurso educationOrganization</span><span class="sxs-lookup"><span data-stu-id="71905-101">educationOrganization resource type</span></span>

<span data-ttu-id="71905-102">Entidade abstrata usada para modelar o que há de comum entre tipos diferentes de organização dentro do setor de educação.</span><span class="sxs-lookup"><span data-stu-id="71905-102">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="71905-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71905-103">Properties</span></span>
| <span data-ttu-id="71905-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71905-104">Property</span></span>     | <span data-ttu-id="71905-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="71905-105">Type</span></span>   |<span data-ttu-id="71905-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="71905-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71905-107">descrição</span><span class="sxs-lookup"><span data-stu-id="71905-107">description</span></span>|<span data-ttu-id="71905-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71905-108">String</span></span>| <span data-ttu-id="71905-109">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="71905-109">Organization description.</span></span>|
|<span data-ttu-id="71905-110">displayName</span><span class="sxs-lookup"><span data-stu-id="71905-110">displayName</span></span>|<span data-ttu-id="71905-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71905-111">String</span></span>| <span data-ttu-id="71905-112">Nome para exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="71905-112">Organization display name.</span></span>|
|<span data-ttu-id="71905-113">externalSource</span><span class="sxs-lookup"><span data-stu-id="71905-113">externalSource</span></span>|<span data-ttu-id="71905-114">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="71905-114">educationExternalSource</span></span>| <span data-ttu-id="71905-115">Fonte a partir da qual esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="71905-115">Source where this organization was created from.</span></span> <span data-ttu-id="71905-116">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="71905-116">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="71905-117">Relações</span><span class="sxs-lookup"><span data-stu-id="71905-117">Relationships</span></span>
<span data-ttu-id="71905-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71905-118">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="71905-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71905-119">JSON representation</span></span>

<span data-ttu-id="71905-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71905-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->