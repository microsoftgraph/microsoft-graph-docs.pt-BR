# <a name="attachment-resource-type"></a><span data-ttu-id="20b59-101">tipo de recurso attachment</span><span class="sxs-lookup"><span data-stu-id="20b59-101">attachment resource type</span></span>

<span data-ttu-id="20b59-102">Você pode adicionar conteúdo relacionado a um [event](../resources/event.md), [message](../resources/message.md) u [post](../resources/post.md) na forma de anexo</span><span class="sxs-lookup"><span data-stu-id="20b59-102">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="20b59-103">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="20b59-103">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="20b59-104">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="20b59-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="20b59-105">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="20b59-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="20b59-106">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceAttachment.md))</span><span class="sxs-lookup"><span data-stu-id="20b59-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="20b59-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="20b59-107">Methods</span></span>

<span data-ttu-id="20b59-108">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="20b59-108">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="20b59-109">Método</span><span class="sxs-lookup"><span data-stu-id="20b59-109">Method</span></span>       | <span data-ttu-id="20b59-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="20b59-110">Return Type</span></span>  |<span data-ttu-id="20b59-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="20b59-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20b59-112">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="20b59-112">Get attachment</span></span>](../api/attachment_get.md) | [<span data-ttu-id="20b59-113">attachment</span><span class="sxs-lookup"><span data-stu-id="20b59-113">attachment</span></span>](attachment.md) |<span data-ttu-id="20b59-114">Leia as propriedades e as relações de um anexo, anexados a um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="20b59-114">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="20b59-115">Adicionar anexo a um event</span><span class="sxs-lookup"><span data-stu-id="20b59-115">Add attachment to an event</span></span>](../api/event_post_attachments.md) | [<span data-ttu-id="20b59-116">attachment</span><span class="sxs-lookup"><span data-stu-id="20b59-116">attachment</span></span>](attachment.md) |<span data-ttu-id="20b59-117">Adicione um arquivo, item ou anexo de link a um evento.</span><span class="sxs-lookup"><span data-stu-id="20b59-117">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="20b59-118">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="20b59-118">Add attachment to a message</span></span>](../api/message_post_attachments.md) | [<span data-ttu-id="20b59-119">attachment</span><span class="sxs-lookup"><span data-stu-id="20b59-119">attachment</span></span>](attachment.md) |<span data-ttu-id="20b59-120">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="20b59-120">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="20b59-121">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="20b59-121">Add attachment to a post</span></span>](../api/post_post_attachments.md) | [<span data-ttu-id="20b59-122">attachment</span><span class="sxs-lookup"><span data-stu-id="20b59-122">attachment</span></span>](attachment.md) |<span data-ttu-id="20b59-123">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="20b59-123">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="20b59-124">Listar anexos de um evento</span><span class="sxs-lookup"><span data-stu-id="20b59-124">List attachments of an event</span></span>](../api/event_list_attachments.md) | <span data-ttu-id="20b59-125">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="20b59-125">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="20b59-126">Obtenha uma lista de anexos de um evento.</span><span class="sxs-lookup"><span data-stu-id="20b59-126">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="20b59-127">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="20b59-127">List attachments of a message</span></span>](../api/message_list_attachments.md) | <span data-ttu-id="20b59-128">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="20b59-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="20b59-129">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="20b59-129">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="20b59-130">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="20b59-130">List attachments of a post</span></span>](../api/post_list_attachments.md) | <span data-ttu-id="20b59-131">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="20b59-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="20b59-132">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="20b59-132">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="20b59-133">Delete</span><span class="sxs-lookup"><span data-stu-id="20b59-133">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="20b59-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20b59-134">None</span></span> |<span data-ttu-id="20b59-135">Exclua um anexo em um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="20b59-135">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="20b59-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20b59-136">Properties</span></span>

<span data-ttu-id="20b59-p101">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceAttachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="20b59-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceAttachment.md)) for additional properties.</span></span>

| <span data-ttu-id="20b59-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20b59-139">Property</span></span>     | <span data-ttu-id="20b59-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="20b59-140">Type</span></span>   |<span data-ttu-id="20b59-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="20b59-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20b59-142">contentType</span><span class="sxs-lookup"><span data-stu-id="20b59-142">contentType</span></span>|<span data-ttu-id="20b59-143">String</span><span class="sxs-lookup"><span data-stu-id="20b59-143">String</span></span>|<span data-ttu-id="20b59-144">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="20b59-144">The MIME type.</span></span>|
|<span data-ttu-id="20b59-145">id</span><span class="sxs-lookup"><span data-stu-id="20b59-145">id</span></span>|<span data-ttu-id="20b59-146">String</span><span class="sxs-lookup"><span data-stu-id="20b59-146">String</span></span>| <span data-ttu-id="20b59-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20b59-147">Read-only.</span></span>|
|<span data-ttu-id="20b59-148">isInline</span><span class="sxs-lookup"><span data-stu-id="20b59-148">isInline</span></span>|<span data-ttu-id="20b59-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="20b59-149">Boolean</span></span>|<span data-ttu-id="20b59-150">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="20b59-150">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="20b59-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20b59-151">lastModifiedDateTime</span></span>|<span data-ttu-id="20b59-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20b59-152">DateTimeOffset</span></span>|<span data-ttu-id="20b59-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="20b59-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="20b59-155">nome</span><span class="sxs-lookup"><span data-stu-id="20b59-155">name</span></span>|<span data-ttu-id="20b59-156">String</span><span class="sxs-lookup"><span data-stu-id="20b59-156">String</span></span>|<span data-ttu-id="20b59-157">Nome de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="20b59-157">The attachment's file name.</span></span>|
|<span data-ttu-id="20b59-158">size</span><span class="sxs-lookup"><span data-stu-id="20b59-158">size</span></span>|<span data-ttu-id="20b59-159">Int32</span><span class="sxs-lookup"><span data-stu-id="20b59-159">Int32</span></span>|<span data-ttu-id="20b59-160">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="20b59-160">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20b59-161">Relações</span><span class="sxs-lookup"><span data-stu-id="20b59-161">Relationships</span></span>
<span data-ttu-id="20b59-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20b59-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20b59-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20b59-163">JSON representation</span></span>

<span data-ttu-id="20b59-164">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="20b59-164">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
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
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
