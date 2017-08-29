# <a name="referenceattachment-resource-type"></a><span data-ttu-id="477f8-101">Tipo de recurso referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="477f8-101">referenceAttachment resource type</span></span>

<span data-ttu-id="477f8-102">Um link para um arquivo (como um arquivo de texto ou um documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento compatíveis, anexado a um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="477f8-102">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="477f8-103">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="477f8-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="477f8-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="477f8-104">Methods</span></span>

| <span data-ttu-id="477f8-105">Método</span><span class="sxs-lookup"><span data-stu-id="477f8-105">Method</span></span>       | <span data-ttu-id="477f8-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="477f8-106">Return Type</span></span>  |<span data-ttu-id="477f8-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="477f8-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="477f8-108">Get</span><span class="sxs-lookup"><span data-stu-id="477f8-108">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="477f8-109">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="477f8-109">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="477f8-110">Leia as propriedades e os relacionamentos do objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="477f8-110">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="477f8-111">Delete</span><span class="sxs-lookup"><span data-stu-id="477f8-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="477f8-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="477f8-112">None</span></span> |<span data-ttu-id="477f8-113">Exclua o objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="477f8-113">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="477f8-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="477f8-114">Properties</span></span>
| <span data-ttu-id="477f8-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="477f8-115">Property</span></span>     | <span data-ttu-id="477f8-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="477f8-116">Type</span></span>   |<span data-ttu-id="477f8-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="477f8-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="477f8-118">contentType</span><span class="sxs-lookup"><span data-stu-id="477f8-118">contentType</span></span>|<span data-ttu-id="477f8-119">String</span><span class="sxs-lookup"><span data-stu-id="477f8-119">String</span></span>|<span data-ttu-id="477f8-120">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="477f8-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="477f8-121">id</span><span class="sxs-lookup"><span data-stu-id="477f8-121">id</span></span>|<span data-ttu-id="477f8-122">String</span><span class="sxs-lookup"><span data-stu-id="477f8-122">String</span></span>|<span data-ttu-id="477f8-p101">A ID do anexo.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="477f8-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="477f8-125">isInline</span><span class="sxs-lookup"><span data-stu-id="477f8-125">isInline</span></span>|<span data-ttu-id="477f8-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="477f8-126">Boolean</span></span>|<span data-ttu-id="477f8-127">Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação.</span><span class="sxs-lookup"><span data-stu-id="477f8-127">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="477f8-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="477f8-128">lastModifiedDateTime</span></span>|<span data-ttu-id="477f8-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="477f8-129">DateTimeOffset</span></span>|<span data-ttu-id="477f8-p102">Data e hora em que o anexo foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="477f8-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="477f8-133">nome</span><span class="sxs-lookup"><span data-stu-id="477f8-133">name</span></span>|<span data-ttu-id="477f8-134">String</span><span class="sxs-lookup"><span data-stu-id="477f8-134">String</span></span>|<span data-ttu-id="477f8-p103">O texto exibido abaixo do ícone que representa o anexo incorporado. Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="477f8-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="477f8-137">size</span><span class="sxs-lookup"><span data-stu-id="477f8-137">size</span></span>|<span data-ttu-id="477f8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="477f8-138">Int32</span></span>|<span data-ttu-id="477f8-139">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="477f8-139">The size of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="477f8-140">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="477f8-140">Relationships</span></span>
<span data-ttu-id="477f8-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="477f8-141">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="477f8-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="477f8-142">JSON representation</span></span>

<span data-ttu-id="477f8-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="477f8-143">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
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
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
