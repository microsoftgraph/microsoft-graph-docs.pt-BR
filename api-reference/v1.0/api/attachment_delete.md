# <a name="delete-attachment"></a><span data-ttu-id="b07ca-101">Excluir anexo</span><span class="sxs-lookup"><span data-stu-id="b07ca-101">Delete attachment</span></span>

<span data-ttu-id="b07ca-102">Exclua um anexo de um evento de calendário, email ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="b07ca-102">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="b07ca-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b07ca-103">Permissions</span></span>
<span data-ttu-id="b07ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b07ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="b07ca-106">Se estiver acessando anexos em Mensagens: Mail.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b07ca-106">If accessing attachments in Messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="b07ca-107">Se estiver acessando anexos em Eventos: Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b07ca-107">If accessing attachments in Events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="b07ca-108">Se estiver acessando anexos em Eventos de grupo ou Postagens: Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="b07ca-108">If accessing attachments in Group Events or Posts: Group.ReadWrite.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="b07ca-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b07ca-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b07ca-110">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="b07ca-110">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
DELETE /groups/{id}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
```
<span data-ttu-id="b07ca-111">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="b07ca-111">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="b07ca-112">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b07ca-112">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="b07ca-113">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="b07ca-113">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b07ca-114">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b07ca-114">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b07ca-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="b07ca-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="b07ca-117">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="b07ca-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b07ca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b07ca-118">Request headers</span></span>
| <span data-ttu-id="b07ca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b07ca-119">Name</span></span>       | <span data-ttu-id="b07ca-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b07ca-120">Type</span></span> | <span data-ttu-id="b07ca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b07ca-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b07ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b07ca-122">Authorization</span></span>  | <span data-ttu-id="b07ca-123">string</span><span class="sxs-lookup"><span data-stu-id="b07ca-123">string</span></span>  | <span data-ttu-id="b07ca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b07ca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b07ca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b07ca-126">Request body</span></span>
<span data-ttu-id="b07ca-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b07ca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b07ca-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b07ca-128">Response</span></span>

<span data-ttu-id="b07ca-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b07ca-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b07ca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b07ca-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b07ca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b07ca-132">Request</span></span>
<span data-ttu-id="b07ca-133">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="b07ca-133">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="b07ca-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b07ca-134">Response</span></span>
<span data-ttu-id="b07ca-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b07ca-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
