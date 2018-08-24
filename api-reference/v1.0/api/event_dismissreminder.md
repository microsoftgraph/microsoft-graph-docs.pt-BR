# <a name="event-dismissreminder"></a><span data-ttu-id="263b8-101">evento: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="263b8-101">event: dismissReminder</span></span>

<span data-ttu-id="263b8-102">Descarte um lembrete disparado em um [evento](../resources/event.md) no [calendário](../resources/calendar.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="263b8-102">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="263b8-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="263b8-103">Permissions</span></span>
<span data-ttu-id="263b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="263b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="263b8-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="263b8-106">Permission type</span></span>      | <span data-ttu-id="263b8-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="263b8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="263b8-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="263b8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="263b8-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="263b8-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="263b8-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="263b8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="263b8-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="263b8-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="263b8-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="263b8-112">Application</span></span> | <span data-ttu-id="263b8-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="263b8-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="263b8-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="263b8-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="263b8-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="263b8-115">Request headers</span></span>
| <span data-ttu-id="263b8-116">Nome</span><span class="sxs-lookup"><span data-stu-id="263b8-116">Name</span></span>       | <span data-ttu-id="263b8-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="263b8-117">Type</span></span> | <span data-ttu-id="263b8-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="263b8-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="263b8-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="263b8-119">Authorization</span></span>  | <span data-ttu-id="263b8-120">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="263b8-120">string</span></span>  | <span data-ttu-id="263b8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="263b8-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="263b8-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="263b8-123">Response</span></span>

<span data-ttu-id="263b8-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="263b8-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="263b8-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="263b8-126">Example</span></span>

<span data-ttu-id="263b8-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="263b8-127">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="263b8-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="263b8-128">Request</span></span>
<span data-ttu-id="263b8-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="263b8-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="263b8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="263b8-130">Response</span></span>
<span data-ttu-id="263b8-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="263b8-131">Here is an example of the response.</span></span>

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
