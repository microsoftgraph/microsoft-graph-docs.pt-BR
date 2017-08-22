# <a name="event-snoozereminder"></a><span data-ttu-id="c7c2e-101">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="c7c2e-101">event: snoozeReminder</span></span>

<span data-ttu-id="c7c2e-102">Adia um lembrete para um novo horário.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-102">Postpone a reminder until a new time.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7c2e-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7c2e-103">Prerequisites</span></span>
<span data-ttu-id="c7c2e-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="c7c2e-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="c7c2e-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7c2e-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder
POST /groups/{id}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder
POST /groups/{id}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="c7c2e-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c2e-106">Request headers</span></span>
| <span data-ttu-id="c7c2e-107">Nome</span><span class="sxs-lookup"><span data-stu-id="c7c2e-107">Name</span></span>       | <span data-ttu-id="c7c2e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7c2e-108">Type</span></span> | <span data-ttu-id="c7c2e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7c2e-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c7c2e-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7c2e-110">Authorization</span></span>  | <span data-ttu-id="c7c2e-111">string</span><span class="sxs-lookup"><span data-stu-id="c7c2e-111">string</span></span>  | <span data-ttu-id="c7c2e-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7c2e-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7c2e-114">Content-Type</span></span> | <span data-ttu-id="c7c2e-115">string</span><span class="sxs-lookup"><span data-stu-id="c7c2e-115">string</span></span>  | <span data-ttu-id="c7c2e-p102">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7c2e-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c2e-118">Request body</span></span>
<span data-ttu-id="c7c2e-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c7c2e-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c7c2e-120">Parameter</span></span>    | <span data-ttu-id="c7c2e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7c2e-121">Type</span></span>   |<span data-ttu-id="c7c2e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7c2e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7c2e-123">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="c7c2e-123">newReminderTime</span></span>|<span data-ttu-id="c7c2e-124">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c7c2e-124">DateTimeTimeZone</span></span>|<span data-ttu-id="c7c2e-125">A nova data e hora para disparar o lembrete.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-125">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="c7c2e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7c2e-126">Response</span></span>

<span data-ttu-id="c7c2e-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c2e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7c2e-129">Example</span></span>
<span data-ttu-id="c7c2e-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7c2e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c2e-131">Request</span></span>
<span data-ttu-id="c7c2e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="c7c2e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7c2e-133">Response</span></span>
<span data-ttu-id="c7c2e-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-134">Here is an example of the response.</span></span>
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
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
