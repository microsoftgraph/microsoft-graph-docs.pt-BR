# <a name="fileattachment-resource-type"></a><span data-ttu-id="11596-101">tipo de recurso fileAttachment</span><span class="sxs-lookup"><span data-stu-id="11596-101">fileAttachment resource type</span></span>

<span data-ttu-id="11596-p101">Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento, mensagem ou postagem. A propriedade **contentBytes** contém os conteúdos com codificação base64 do arquivo.</span><span class="sxs-lookup"><span data-stu-id="11596-p101">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="11596-104">Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="11596-104">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="11596-105">As propriedades **name** e **contentBytes** necessárias.</span><span class="sxs-lookup"><span data-stu-id="11596-105">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="11596-106">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="11596-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="11596-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="11596-107">Methods</span></span>

| <span data-ttu-id="11596-108">Método</span><span class="sxs-lookup"><span data-stu-id="11596-108">Method</span></span>       | <span data-ttu-id="11596-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="11596-109">Return Type</span></span>  |<span data-ttu-id="11596-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11596-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11596-111">Get</span><span class="sxs-lookup"><span data-stu-id="11596-111">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="11596-112">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="11596-112">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="11596-113">Leia as propriedades e os relacionamentos do objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="11596-113">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="11596-114">Delete</span><span class="sxs-lookup"><span data-stu-id="11596-114">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="11596-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="11596-115">None</span></span> |<span data-ttu-id="11596-116">Exclua um objeto fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="11596-116">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="11596-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11596-117">Properties</span></span>
| <span data-ttu-id="11596-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11596-118">Property</span></span>     | <span data-ttu-id="11596-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="11596-119">Type</span></span>   |<span data-ttu-id="11596-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="11596-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11596-121">contentBytes</span><span class="sxs-lookup"><span data-stu-id="11596-121">contentBytes</span></span>|<span data-ttu-id="11596-122">Binário</span><span class="sxs-lookup"><span data-stu-id="11596-122">Binary</span></span>|<span data-ttu-id="11596-123">O conteúdo binário do arquivo.</span><span class="sxs-lookup"><span data-stu-id="11596-123">The binary contents of the file.</span></span>|
|<span data-ttu-id="11596-124">contentId</span><span class="sxs-lookup"><span data-stu-id="11596-124">contentId</span></span>|<span data-ttu-id="11596-125">String</span><span class="sxs-lookup"><span data-stu-id="11596-125">String</span></span>|<span data-ttu-id="11596-126">A ID do anexo no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="11596-126">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="11596-127">contentLocation</span><span class="sxs-lookup"><span data-stu-id="11596-127">contentLocation</span></span>|<span data-ttu-id="11596-128">String</span><span class="sxs-lookup"><span data-stu-id="11596-128">String</span></span>|<span data-ttu-id="11596-129">O URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="11596-129">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="11596-130">contentType</span><span class="sxs-lookup"><span data-stu-id="11596-130">contentType</span></span>|<span data-ttu-id="11596-131">String</span><span class="sxs-lookup"><span data-stu-id="11596-131">String</span></span>|<span data-ttu-id="11596-132">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="11596-132">The content type of the attachment.</span></span>|
|<span data-ttu-id="11596-133">id</span><span class="sxs-lookup"><span data-stu-id="11596-133">id</span></span>|<span data-ttu-id="11596-134">String</span><span class="sxs-lookup"><span data-stu-id="11596-134">String</span></span>|<span data-ttu-id="11596-135">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="11596-135">The attachment ID.</span></span>|
|<span data-ttu-id="11596-136">isInline</span><span class="sxs-lookup"><span data-stu-id="11596-136">isInline</span></span>|<span data-ttu-id="11596-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="11596-137">Boolean</span></span>|<span data-ttu-id="11596-138">Defina como true se este for um anexo embutido.</span><span class="sxs-lookup"><span data-stu-id="11596-138">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="11596-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11596-139">lastModifiedDateTime</span></span>|<span data-ttu-id="11596-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11596-140">DateTimeOffset</span></span>|<span data-ttu-id="11596-141">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="11596-141">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="11596-142">name</span><span class="sxs-lookup"><span data-stu-id="11596-142">name</span></span>|<span data-ttu-id="11596-143">String</span><span class="sxs-lookup"><span data-stu-id="11596-143">String</span></span>|<span data-ttu-id="11596-144">O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="11596-144">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="11596-145">size</span><span class="sxs-lookup"><span data-stu-id="11596-145">size</span></span>|<span data-ttu-id="11596-146">Int32</span><span class="sxs-lookup"><span data-stu-id="11596-146">Int32</span></span>|<span data-ttu-id="11596-147">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="11596-147">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11596-148">Relações</span><span class="sxs-lookup"><span data-stu-id="11596-148">Relationships</span></span>
<span data-ttu-id="11596-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11596-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="11596-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11596-150">JSON representation</span></span>

<span data-ttu-id="11596-151">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="11596-151">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
  "contentId": "string",
  "contentLocation": "string",
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
