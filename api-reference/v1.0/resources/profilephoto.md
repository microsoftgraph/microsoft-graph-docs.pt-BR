# <a name="profilephoto-resource-type"></a><span data-ttu-id="64e62-101">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="64e62-101">profilePhoto resource type</span></span>
<span data-ttu-id="64e62-p101">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.</span><span class="sxs-lookup"><span data-stu-id="64e62-p101">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="64e62-104">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="64e62-104">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="64e62-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="64e62-105">Methods</span></span>

| <span data-ttu-id="64e62-106">Método</span><span class="sxs-lookup"><span data-stu-id="64e62-106">Method</span></span>       | <span data-ttu-id="64e62-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="64e62-107">Return Type</span></span>  |<span data-ttu-id="64e62-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="64e62-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64e62-109">Obter profilePhoto</span><span class="sxs-lookup"><span data-stu-id="64e62-109">Get profilePhoto</span></span>](../api/profilephoto_get.md) | [<span data-ttu-id="64e62-110">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="64e62-110">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="64e62-111">Obtenha a **profilePhoto** especificada ou seus metadados (propriedades de profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="64e62-111">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="64e62-112">Atualizar</span><span class="sxs-lookup"><span data-stu-id="64e62-112">Update</span></span>](../api/profilephoto_update.md) | [<span data-ttu-id="64e62-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="64e62-113">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="64e62-p102">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="64e62-p102">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="64e62-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64e62-117">Properties</span></span>
| <span data-ttu-id="64e62-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64e62-118">Property</span></span>     | <span data-ttu-id="64e62-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="64e62-119">Type</span></span>   |<span data-ttu-id="64e62-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="64e62-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64e62-121">id</span><span class="sxs-lookup"><span data-stu-id="64e62-121">id</span></span>|<span data-ttu-id="64e62-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e62-122">string</span></span>|<span data-ttu-id="64e62-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64e62-123">Read-only.</span></span>|
|<span data-ttu-id="64e62-124">height</span><span class="sxs-lookup"><span data-stu-id="64e62-124">height</span></span>|<span data-ttu-id="64e62-125">int32</span><span class="sxs-lookup"><span data-stu-id="64e62-125">int32</span></span>|<span data-ttu-id="64e62-p103">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64e62-p103">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="64e62-128">width</span><span class="sxs-lookup"><span data-stu-id="64e62-128">width</span></span>|<span data-ttu-id="64e62-129">int32</span><span class="sxs-lookup"><span data-stu-id="64e62-129">int32</span></span>|<span data-ttu-id="64e62-p104">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64e62-p104">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64e62-132">Relações</span><span class="sxs-lookup"><span data-stu-id="64e62-132">Relationships</span></span>
<span data-ttu-id="64e62-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64e62-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="64e62-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64e62-134">JSON representation</span></span>

<span data-ttu-id="64e62-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64e62-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
