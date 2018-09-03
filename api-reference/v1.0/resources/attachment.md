# <a name="attachment-resource-type"></a><span data-ttu-id="64701-101">tipo de recurso attachment</span><span class="sxs-lookup"><span data-stu-id="64701-101">attachment resource type</span></span>

<span data-ttu-id="64701-102">Você pode adicionar conteúdo relacionado a um [event](../resources/event.md), [message](../resources/message.md) u [post](../resources/post.md) na forma de anexo</span><span class="sxs-lookup"><span data-stu-id="64701-102">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="64701-103">**attachment** é o recurso de base para os seguintes tipos de anexo derivados:</span><span class="sxs-lookup"><span data-stu-id="64701-103">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="64701-104">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))</span><span class="sxs-lookup"><span data-stu-id="64701-104">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="64701-105">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))</span><span class="sxs-lookup"><span data-stu-id="64701-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="64701-106">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceAttachment.md))</span><span class="sxs-lookup"><span data-stu-id="64701-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="64701-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="64701-107">Methods</span></span>

<span data-ttu-id="64701-108">Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="64701-108">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="64701-109">Método</span><span class="sxs-lookup"><span data-stu-id="64701-109">Method</span></span>       | <span data-ttu-id="64701-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="64701-110">Return Type</span></span>  |<span data-ttu-id="64701-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="64701-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64701-112">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="64701-112">Get attachment</span></span>](../api/attachment_get.md) | [<span data-ttu-id="64701-113">attachment</span><span class="sxs-lookup"><span data-stu-id="64701-113">attachment</span></span>](attachment.md) |<span data-ttu-id="64701-114">Leia as propriedades e as relações de um anexo, anexados a um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="64701-114">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="64701-115">Adicionar anexo a um event</span><span class="sxs-lookup"><span data-stu-id="64701-115">Add attachment to an event</span></span>](../api/event_post_attachments.md) | [<span data-ttu-id="64701-116">attachment</span><span class="sxs-lookup"><span data-stu-id="64701-116">attachment</span></span>](attachment.md) |<span data-ttu-id="64701-117">Adicione um arquivo, item ou anexo de link a um evento.</span><span class="sxs-lookup"><span data-stu-id="64701-117">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="64701-118">Adicionar um anexo a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="64701-118">Add attachment to a message</span></span>](../api/message_post_attachments.md) | [<span data-ttu-id="64701-119">attachment</span><span class="sxs-lookup"><span data-stu-id="64701-119">attachment</span></span>](attachment.md) |<span data-ttu-id="64701-120">Adicione um arquivo, item ou anexo de link a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="64701-120">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="64701-121">Adicionar anexo a uma postagem</span><span class="sxs-lookup"><span data-stu-id="64701-121">Add attachment to a post</span></span>](../api/post_post_attachments.md) | [<span data-ttu-id="64701-122">attachment</span><span class="sxs-lookup"><span data-stu-id="64701-122">attachment</span></span>](attachment.md) |<span data-ttu-id="64701-123">Adicione um arquivo, item ou anexo de link a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="64701-123">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="64701-124">Listar anexos de um evento</span><span class="sxs-lookup"><span data-stu-id="64701-124">List attachments of an event</span></span>](../api/event_list_attachments.md) | <span data-ttu-id="64701-125">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="64701-125">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="64701-126">Obtenha uma lista de anexos de um evento.</span><span class="sxs-lookup"><span data-stu-id="64701-126">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="64701-127">Listar anexos de uma mensagem</span><span class="sxs-lookup"><span data-stu-id="64701-127">List attachments of a message</span></span>](../api/message_list_attachments.md) | <span data-ttu-id="64701-128">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="64701-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="64701-129">Obtenha uma lista de anexos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="64701-129">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="64701-130">Listar anexos de uma postagem</span><span class="sxs-lookup"><span data-stu-id="64701-130">List attachments of a post</span></span>](../api/post_list_attachments.md) | <span data-ttu-id="64701-131">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="64701-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="64701-132">Obtenha uma lista de anexos de uma postagem.</span><span class="sxs-lookup"><span data-stu-id="64701-132">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="64701-133">Excluir</span><span class="sxs-lookup"><span data-stu-id="64701-133">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="64701-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64701-134">None</span></span> |<span data-ttu-id="64701-135">Exclua um anexo em um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="64701-135">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="64701-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64701-136">Properties</span></span>

<span data-ttu-id="64701-p101">A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceAttachment.md)) para propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="64701-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceAttachment.md)) for additional properties.</span></span>

| <span data-ttu-id="64701-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64701-139">Property</span></span>     | <span data-ttu-id="64701-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="64701-140">Type</span></span>   |<span data-ttu-id="64701-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="64701-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64701-142">contentType</span><span class="sxs-lookup"><span data-stu-id="64701-142">contentType</span></span>|<span data-ttu-id="64701-143">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="64701-143">String</span></span>|<span data-ttu-id="64701-144">O tipo MIME.</span><span class="sxs-lookup"><span data-stu-id="64701-144">The MIME type.</span></span>|
|<span data-ttu-id="64701-145">id</span><span class="sxs-lookup"><span data-stu-id="64701-145">id</span></span>|<span data-ttu-id="64701-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64701-146">String</span></span>| <span data-ttu-id="64701-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64701-147">Read-only.</span></span>|
|<span data-ttu-id="64701-148">isInline</span><span class="sxs-lookup"><span data-stu-id="64701-148">isInline</span></span>|<span data-ttu-id="64701-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="64701-149">Boolean</span></span>|<span data-ttu-id="64701-150">`true` se o anexo for embutido; caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="64701-150">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="64701-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64701-151">lastModifiedDateTime</span></span>|<span data-ttu-id="64701-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64701-152">DateTimeOffset</span></span>|<span data-ttu-id="64701-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="64701-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="64701-155">nome</span><span class="sxs-lookup"><span data-stu-id="64701-155">name</span></span>|<span data-ttu-id="64701-156">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="64701-156">String</span></span>|<span data-ttu-id="64701-157">Nome de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="64701-157">The attachment's file name.</span></span>|
|<span data-ttu-id="64701-158">size</span><span class="sxs-lookup"><span data-stu-id="64701-158">size</span></span>|<span data-ttu-id="64701-159">Int32</span><span class="sxs-lookup"><span data-stu-id="64701-159">Int32</span></span>|<span data-ttu-id="64701-160">O comprimento do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="64701-160">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64701-161">Relações</span><span class="sxs-lookup"><span data-stu-id="64701-161">Relationships</span></span>
<span data-ttu-id="64701-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64701-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64701-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64701-163">JSON representation</span></span>

<span data-ttu-id="64701-164">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="64701-164">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
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
