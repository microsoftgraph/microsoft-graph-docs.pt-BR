# <a name="event-tentativelyaccept"></a><span data-ttu-id="71d69-101">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="71d69-101">event: tentativelyAccept</span></span>

<span data-ttu-id="71d69-102">Aceita provisoriamente o evento especificado.</span><span class="sxs-lookup"><span data-stu-id="71d69-102">Tentatively accept the specified event.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71d69-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71d69-103">Prerequisites</span></span>
<span data-ttu-id="71d69-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="71d69-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="71d69-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71d69-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept
POST /groups/{id}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept
POST /groups/{id}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="71d69-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71d69-106">Request headers</span></span>
| <span data-ttu-id="71d69-107">Nome</span><span class="sxs-lookup"><span data-stu-id="71d69-107">Name</span></span>       | <span data-ttu-id="71d69-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="71d69-108">Type</span></span> | <span data-ttu-id="71d69-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="71d69-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71d69-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="71d69-110">Authorization</span></span>  | <span data-ttu-id="71d69-111">string</span><span class="sxs-lookup"><span data-stu-id="71d69-111">string</span></span>  | <span data-ttu-id="71d69-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71d69-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71d69-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71d69-114">Content-Type</span></span> | <span data-ttu-id="71d69-115">string</span><span class="sxs-lookup"><span data-stu-id="71d69-115">string</span></span>  | <span data-ttu-id="71d69-p102">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71d69-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71d69-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71d69-118">Request body</span></span>
<span data-ttu-id="71d69-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71d69-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71d69-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="71d69-120">Parameter</span></span>    | <span data-ttu-id="71d69-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="71d69-121">Type</span></span>   |<span data-ttu-id="71d69-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="71d69-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71d69-123">comment</span><span class="sxs-lookup"><span data-stu-id="71d69-123">comment</span></span>|<span data-ttu-id="71d69-124">String</span><span class="sxs-lookup"><span data-stu-id="71d69-124">String</span></span>|<span data-ttu-id="71d69-p103">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="71d69-p103">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="71d69-127">sendResponse</span><span class="sxs-lookup"><span data-stu-id="71d69-127">sendResponse</span></span>|<span data-ttu-id="71d69-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="71d69-128">Boolean</span></span>|<span data-ttu-id="71d69-p104">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="71d69-p104">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="71d69-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="71d69-132">Response</span></span>

<span data-ttu-id="71d69-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71d69-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71d69-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71d69-135">Example</span></span>
<span data-ttu-id="71d69-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="71d69-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="71d69-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71d69-137">Request</span></span>
<span data-ttu-id="71d69-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71d69-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="71d69-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="71d69-139">Response</span></span>
##### <a name="response"></a><span data-ttu-id="71d69-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="71d69-140">Response</span></span>
<span data-ttu-id="71d69-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71d69-141">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
