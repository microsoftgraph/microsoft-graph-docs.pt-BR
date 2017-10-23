# <a name="add-attachment"></a><span data-ttu-id="b1956-101">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="b1956-101">Add attachment</span></span>

<span data-ttu-id="b1956-p101">Use esta API para adicionar um [anexo](../resources/attachment.md) a um evento. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="b1956-p101">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1956-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1956-104">Permissions</span></span>
<span data-ttu-id="b1956-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1956-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1956-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1956-107">Permission type</span></span>      | <span data-ttu-id="b1956-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1956-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1956-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1956-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b1956-110">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1956-110">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b1956-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1956-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1956-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1956-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b1956-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1956-113">Application</span></span> | <span data-ttu-id="b1956-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1956-114">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1956-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1956-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b1956-116">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="b1956-116">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
POST /groups/{id}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
```
<span data-ttu-id="b1956-117">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="b1956-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="b1956-118">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b1956-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="b1956-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1956-119">Request headers</span></span>
| <span data-ttu-id="b1956-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b1956-120">Name</span></span>       | <span data-ttu-id="b1956-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1956-121">Type</span></span> | <span data-ttu-id="b1956-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1956-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b1956-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1956-123">Authorization</span></span>  | <span data-ttu-id="b1956-124">string</span><span class="sxs-lookup"><span data-stu-id="b1956-124">string</span></span>  | <span data-ttu-id="b1956-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1956-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1956-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1956-127">Content-Type</span></span> | <span data-ttu-id="b1956-128">string</span><span class="sxs-lookup"><span data-stu-id="b1956-128">string</span></span>  | <span data-ttu-id="b1956-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1956-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1956-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1956-131">Request body</span></span>
<span data-ttu-id="b1956-132">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b1956-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b1956-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1956-133">Response</span></span>

<span data-ttu-id="b1956-134">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1956-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="b1956-135">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="b1956-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="b1956-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1956-136">Request</span></span>
<span data-ttu-id="b1956-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1956-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments 
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```

<span data-ttu-id="b1956-138">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b1956-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="b1956-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1956-139">Response</span></span>
<span data-ttu-id="b1956-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1956-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-Length: 735

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="b1956-141">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="b1956-141">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="b1956-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1956-142">Request</span></span>

<span data-ttu-id="b1956-143">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="b1956-143">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
Content-type: application/json
Content-length: 600

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
        "@odata.type": "microsoft.graph.event",
        "subject": "Discuss gifts for children",
        "body": {
            "contentType": "HTML",
            "content": "Let's look for funding!"
         },
         "start": {
             "dateTime": "2016-12-02T18:00:00",
             "timeZone": "Pacific Standard Time"
          },
          "end": {
             "dateTime": "2016-12-02T19:00:00",
             "timeZone": "Pacific Standard Time"
          }
    }
}
```

##### <a name="response"></a><span data-ttu-id="b1956-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1956-144">Response</span></span>
<span data-ttu-id="b1956-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1956-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/api/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/api/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
