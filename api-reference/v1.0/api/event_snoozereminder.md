# <a name="event-snoozereminder"></a><span data-ttu-id="b8149-101">evento: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="b8149-101">event: snoozeReminder</span></span>

<span data-ttu-id="b8149-102">Adie um lembrete de um [evento](../resources/event.md) no [calendário](../resources/calendar.md) de um usuário para um novo horário.</span><span class="sxs-lookup"><span data-stu-id="b8149-102">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8149-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8149-103">Permissions</span></span>
<span data-ttu-id="b8149-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8149-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8149-106">Permission type</span></span>      | <span data-ttu-id="b8149-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8149-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8149-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8149-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b8149-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8149-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b8149-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8149-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8149-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8149-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b8149-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8149-112">Application</span></span> | <span data-ttu-id="b8149-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8149-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8149-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8149-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="b8149-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8149-115">Request headers</span></span>
| <span data-ttu-id="b8149-116">Nome</span><span class="sxs-lookup"><span data-stu-id="b8149-116">Name</span></span>       | <span data-ttu-id="b8149-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8149-117">Type</span></span> | <span data-ttu-id="b8149-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8149-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8149-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8149-119">Authorization</span></span>  | <span data-ttu-id="b8149-120">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8149-120">string</span></span>  | <span data-ttu-id="b8149-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8149-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8149-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8149-123">Content-Type</span></span> | <span data-ttu-id="b8149-124">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8149-124">string</span></span>  | <span data-ttu-id="b8149-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8149-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8149-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8149-127">Request body</span></span>
<span data-ttu-id="b8149-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8149-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b8149-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b8149-129">Parameter</span></span>    | <span data-ttu-id="b8149-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8149-130">Type</span></span>   |<span data-ttu-id="b8149-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8149-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8149-132">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="b8149-132">newReminderTime</span></span>|<span data-ttu-id="b8149-133">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b8149-133">DateTimeTimeZone</span></span>|<span data-ttu-id="b8149-134">A nova data e hora para disparar o lembrete.</span><span class="sxs-lookup"><span data-stu-id="b8149-134">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="b8149-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8149-135">Response</span></span>

<span data-ttu-id="b8149-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8149-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8149-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8149-138">Example</span></span>
<span data-ttu-id="b8149-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b8149-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b8149-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8149-140">Request</span></span>
<span data-ttu-id="b8149-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8149-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b8149-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8149-142">Response</span></span>
<span data-ttu-id="b8149-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8149-143">Here is an example of the response.</span></span>
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
