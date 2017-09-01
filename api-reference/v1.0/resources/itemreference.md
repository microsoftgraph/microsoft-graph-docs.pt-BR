# <a name="itemreference-resource-type"></a><span data-ttu-id="ce211-101">Tipo de recurso ItemReference</span><span class="sxs-lookup"><span data-stu-id="ce211-101">ItemReference resource type</span></span>

<span data-ttu-id="ce211-102">O recurso **ItemReference** proporciona as informações necessárias para enviar um [DriveItem](driveitem.md) pela API.</span><span class="sxs-lookup"><span data-stu-id="ce211-102">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce211-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce211-103">JSON representation</span></span>

<span data-ttu-id="ce211-104">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ce211-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="ce211-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce211-105">Properties</span></span>

| <span data-ttu-id="ce211-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce211-106">Property</span></span>      | <span data-ttu-id="ce211-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce211-107">Type</span></span>                              | <span data-ttu-id="ce211-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce211-108">Description</span></span>                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ce211-109">driveId</span><span class="sxs-lookup"><span data-stu-id="ce211-109">driveId</span></span>       | <span data-ttu-id="ce211-110">String</span><span class="sxs-lookup"><span data-stu-id="ce211-110">String</span></span>                            | <span data-ttu-id="ce211-p101">O identificador exclusivo da instância da unidade que contém o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce211-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>                                 |
| <span data-ttu-id="ce211-113">id</span><span class="sxs-lookup"><span data-stu-id="ce211-113">id</span></span>            | <span data-ttu-id="ce211-114">String</span><span class="sxs-lookup"><span data-stu-id="ce211-114">String</span></span>                            | <span data-ttu-id="ce211-p102">Identificador exclusivo do item na unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce211-p102">Unique identifier of the item in the drive. Read-only.</span></span>                                                     |
| <span data-ttu-id="ce211-117">nome</span><span class="sxs-lookup"><span data-stu-id="ce211-117">name</span></span>          | <span data-ttu-id="ce211-118">String</span><span class="sxs-lookup"><span data-stu-id="ce211-118">String</span></span>                            | <span data-ttu-id="ce211-p103">O nome do item ao qual se faz referência. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce211-p103">The name of the item being referenced. Read-only.</span></span>                                                          |
| <span data-ttu-id="ce211-121">caminho</span><span class="sxs-lookup"><span data-stu-id="ce211-121">path</span></span>          | <span data-ttu-id="ce211-122">String</span><span class="sxs-lookup"><span data-stu-id="ce211-122">String</span></span>                            | <span data-ttu-id="ce211-p104">Caminho que pode ser usado para navegar até o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce211-p104">Path that can be used to navigate to the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="ce211-125">shareId</span><span class="sxs-lookup"><span data-stu-id="ce211-125">shareId</span></span>       | <span data-ttu-id="ce211-126">String</span><span class="sxs-lookup"><span data-stu-id="ce211-126">String</span></span>                            | <span data-ttu-id="ce211-127">Um identificador exclusivo para um recurso compartilhado que pode ser acessado através da API [Shares](../api/shares_get.md).</span><span class="sxs-lookup"><span data-stu-id="ce211-127">A unique identifier for a shared resource that can be accessed via the [Shares](../api/shares_get.md) API.</span></span> |
| <span data-ttu-id="ce211-128">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ce211-128">sharepointIds</span></span> | [<span data-ttu-id="ce211-129">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ce211-129">sharepointIds</span></span>](sharepointids.md) | <span data-ttu-id="ce211-p105">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce211-p105">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                   |

## <a name="remarks"></a><span data-ttu-id="ce211-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="ce211-132">Remarks</span></span>

<span data-ttu-id="ce211-133">Para lidar com um **driveItem** de um recurso **itemReference**, crie uma URL no formato:</span><span class="sxs-lookup"><span data-stu-id="ce211-133">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="ce211-134">O valor **path** é um caminho da API relativo à unidade de destino, por exemplo: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="ce211-134">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="ce211-135">Para recuperar o caminho legível para a navegação estrutural, ignore tudo até o primeiro `:` na cadeia de caracteres do caminho.</span><span class="sxs-lookup"><span data-stu-id="ce211-135">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
