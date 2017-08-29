# <a name="sharinglink-resource-type"></a><span data-ttu-id="73334-101">Tipo de recurso SharingLink</span><span class="sxs-lookup"><span data-stu-id="73334-101">SharingLink resource type</span></span>

<span data-ttu-id="73334-102">O recurso **SharingLink** agrupa itens de dados relacionados ao link em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="73334-102">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="73334-103">Se um recurso [**Permission**](permission.md) tiver uma faceta **sharingLink** não nula, a permissão representará um link de compartilhamento (em vez de permissões concedidas a uma pessoa ou um grupo).</span><span class="sxs-lookup"><span data-stu-id="73334-103">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="73334-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73334-104">JSON representation</span></span>

<span data-ttu-id="73334-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73334-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="73334-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73334-106">Properties</span></span>

| <span data-ttu-id="73334-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73334-107">Property</span></span>    | <span data-ttu-id="73334-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="73334-108">Type</span></span>                    | <span data-ttu-id="73334-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73334-109">Description</span></span>                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="73334-110">aplicativo</span><span class="sxs-lookup"><span data-stu-id="73334-110">application</span></span> | [<span data-ttu-id="73334-111">identity</span><span class="sxs-lookup"><span data-stu-id="73334-111">identity</span></span>](identity.md) | <span data-ttu-id="73334-112">O aplicativo ao qual o link está associado.</span><span class="sxs-lookup"><span data-stu-id="73334-112">The app the link is associated with.</span></span>                                                                                                                                                                    |
| <span data-ttu-id="73334-113">type</span><span class="sxs-lookup"><span data-stu-id="73334-113">type</span></span>        | <span data-ttu-id="73334-114">String</span><span class="sxs-lookup"><span data-stu-id="73334-114">String</span></span>                  | <span data-ttu-id="73334-115">O tipo do link criado.</span><span class="sxs-lookup"><span data-stu-id="73334-115">The type of the link created.</span></span>                                                                                                                                                                           |
| <span data-ttu-id="73334-116">scope</span><span class="sxs-lookup"><span data-stu-id="73334-116">scope</span></span>       | <span data-ttu-id="73334-117">String</span><span class="sxs-lookup"><span data-stu-id="73334-117">String</span></span>                  | <span data-ttu-id="73334-p101">O escopo do link representado por esta permissão. O valor `anonymous` indica que o link é utilizável por qualquer pessoa; `organization` indica que o link só é útil para usuários conectados ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="73334-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span> |
| <span data-ttu-id="73334-120">webUrl</span><span class="sxs-lookup"><span data-stu-id="73334-120">webUrl</span></span>      | <span data-ttu-id="73334-121">String</span><span class="sxs-lookup"><span data-stu-id="73334-121">String</span></span>                  | <span data-ttu-id="73334-122">Uma URL que abre o item no navegador no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="73334-122">A URL that opens the item in the browser on the OneDrive website.</span></span>                                                                                                                                       |

## <a name="type-enumeration"></a><span data-ttu-id="73334-123">Enumeração Type</span><span class="sxs-lookup"><span data-stu-id="73334-123">Type enumeration</span></span>

<span data-ttu-id="73334-124">Esta tabela define os valores possíveis para a propriedade **type**:</span><span class="sxs-lookup"><span data-stu-id="73334-124">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="73334-125">Valor</span><span class="sxs-lookup"><span data-stu-id="73334-125">Value</span></span>   | <span data-ttu-id="73334-126">Função</span><span class="sxs-lookup"><span data-stu-id="73334-126">Role</span></span>    | <span data-ttu-id="73334-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="73334-127">Description</span></span>                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | <span data-ttu-id="73334-128">Um link somente de compartilhamento para exibição, permitindo o acesso somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73334-128">A view-only sharing link, allowing read-only access.</span></span>                            |
| `edit`  | `write` | <span data-ttu-id="73334-129">Um link de compartilhamento de edição, permitindo o acesso de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="73334-129">An edit sharing link, allowing read-write access.</span></span>                               |

## <a name="scope-enumeration"></a><span data-ttu-id="73334-130">Enumeração de escopo</span><span class="sxs-lookup"><span data-stu-id="73334-130">Scope enumeration</span></span>

| <span data-ttu-id="73334-131">Valor</span><span class="sxs-lookup"><span data-stu-id="73334-131">Value</span></span>          | <span data-ttu-id="73334-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="73334-132">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="73334-133">O link de compartilhamento está disponível para uso por qualquer pessoa.</span><span class="sxs-lookup"><span data-stu-id="73334-133">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="73334-p102">O link de compartilhamento está disponível para uso por qualquer pessoa na mesma organização (locatário). Não disponível para o OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="73334-p102">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
