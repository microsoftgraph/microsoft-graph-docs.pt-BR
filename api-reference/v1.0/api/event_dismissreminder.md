# <a name="event-dismissreminder"></a><span data-ttu-id="6e183-101">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="6e183-101">event: dismissReminder</span></span>

<span data-ttu-id="6e183-102">Ignorar um lembrete acionado.</span><span class="sxs-lookup"><span data-stu-id="6e183-102">Dissmiss a reminder that has been triggered.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e183-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e183-103">Prerequisites</span></span>
<span data-ttu-id="6e183-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="6e183-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="6e183-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e183-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder
POST /groups/{id}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder
POST /groups/{id}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```
## <a name="request-headers"></a><span data-ttu-id="6e183-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e183-106">Request headers</span></span>
| <span data-ttu-id="6e183-107">Nome</span><span class="sxs-lookup"><span data-stu-id="6e183-107">Name</span></span>       | <span data-ttu-id="6e183-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e183-108">Type</span></span> | <span data-ttu-id="6e183-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e183-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6e183-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e183-110">Authorization</span></span>  | <span data-ttu-id="6e183-111">string</span><span class="sxs-lookup"><span data-stu-id="6e183-111">string</span></span>  | <span data-ttu-id="6e183-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e183-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e183-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e183-114">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6e183-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e183-115">Response</span></span>

<span data-ttu-id="6e183-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e183-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e183-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e183-118">Example</span></span>
<span data-ttu-id="6e183-119">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6e183-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e183-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e183-120">Request</span></span>
<span data-ttu-id="6e183-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e183-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

##### <a name="response"></a><span data-ttu-id="6e183-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e183-122">Response</span></span>
##### <a name="response"></a><span data-ttu-id="6e183-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e183-123">Response</span></span>
<span data-ttu-id="6e183-124">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e183-124">Here is an example of the response.</span></span>
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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
