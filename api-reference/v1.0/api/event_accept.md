# <a name="event-accept"></a><span data-ttu-id="870a2-101">event: accept</span><span class="sxs-lookup"><span data-stu-id="870a2-101">event: accept</span></span>

<span data-ttu-id="870a2-102">Aceita o evento especificado.</span><span class="sxs-lookup"><span data-stu-id="870a2-102">Accept the specified event.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="870a2-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="870a2-103">Prerequisites</span></span>
<span data-ttu-id="870a2-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="870a2-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="870a2-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="870a2-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept
POST /groups/{id}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept
POST /groups/{id}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="870a2-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="870a2-106">Request headers</span></span>
| <span data-ttu-id="870a2-107">Nome</span><span class="sxs-lookup"><span data-stu-id="870a2-107">Name</span></span>       | <span data-ttu-id="870a2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="870a2-108">Type</span></span> | <span data-ttu-id="870a2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="870a2-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="870a2-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="870a2-110">Authorization</span></span>  | <span data-ttu-id="870a2-111">string</span><span class="sxs-lookup"><span data-stu-id="870a2-111">string</span></span>  | <span data-ttu-id="870a2-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="870a2-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="870a2-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="870a2-114">Content-Type</span></span> | <span data-ttu-id="870a2-115">string</span><span class="sxs-lookup"><span data-stu-id="870a2-115">string</span></span>  | <span data-ttu-id="870a2-p102">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="870a2-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="870a2-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="870a2-118">Request body</span></span>
<span data-ttu-id="870a2-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="870a2-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="870a2-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="870a2-120">Parameter</span></span>    | <span data-ttu-id="870a2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="870a2-121">Type</span></span>   |<span data-ttu-id="870a2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="870a2-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="870a2-123">comment</span><span class="sxs-lookup"><span data-stu-id="870a2-123">comment</span></span>|<span data-ttu-id="870a2-124">String</span><span class="sxs-lookup"><span data-stu-id="870a2-124">String</span></span>|<span data-ttu-id="870a2-p103">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="870a2-p103">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="870a2-127">sendResponse</span><span class="sxs-lookup"><span data-stu-id="870a2-127">sendResponse</span></span>|<span data-ttu-id="870a2-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="870a2-128">Boolean</span></span>|<span data-ttu-id="870a2-p104">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="870a2-p104">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="870a2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="870a2-132">Response</span></span>

<span data-ttu-id="870a2-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="870a2-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="870a2-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="870a2-135">Example</span></span>
<span data-ttu-id="870a2-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="870a2-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="870a2-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="870a2-137">Request</span></span>
<span data-ttu-id="870a2-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="870a2-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="870a2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="870a2-139">Response</span></span>
<span data-ttu-id="870a2-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="870a2-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
