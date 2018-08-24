# <a name="event-tentativelyaccept"></a><span data-ttu-id="ab35d-101">evento: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="ab35d-101">event: tentativelyAccept</span></span>

<span data-ttu-id="ab35d-102">Aceite provisoriamente o [evento](../resources/event.md) específico no [calendário](../resources/calendar.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ab35d-102">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab35d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab35d-103">Permissions</span></span>
<span data-ttu-id="ab35d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab35d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab35d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab35d-106">Permission type</span></span>      | <span data-ttu-id="ab35d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab35d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab35d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab35d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ab35d-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab35d-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ab35d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab35d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab35d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab35d-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ab35d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab35d-112">Application</span></span> | <span data-ttu-id="ab35d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab35d-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab35d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab35d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="ab35d-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab35d-115">Request headers</span></span>
| <span data-ttu-id="ab35d-116">Nome</span><span class="sxs-lookup"><span data-stu-id="ab35d-116">Name</span></span>       | <span data-ttu-id="ab35d-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab35d-117">Type</span></span> | <span data-ttu-id="ab35d-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab35d-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ab35d-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab35d-119">Authorization</span></span>  | <span data-ttu-id="ab35d-120">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab35d-120">string</span></span>  | <span data-ttu-id="ab35d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab35d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab35d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab35d-123">Content-Type</span></span> | <span data-ttu-id="ab35d-124">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab35d-124">string</span></span>  | <span data-ttu-id="ab35d-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab35d-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab35d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab35d-127">Request body</span></span>
<span data-ttu-id="ab35d-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab35d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ab35d-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ab35d-129">Parameter</span></span>    | <span data-ttu-id="ab35d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab35d-130">Type</span></span>   |<span data-ttu-id="ab35d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab35d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab35d-132">comentário</span><span class="sxs-lookup"><span data-stu-id="ab35d-132">comment</span></span>|<span data-ttu-id="ab35d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab35d-133">String</span></span>|<span data-ttu-id="ab35d-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ab35d-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="ab35d-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="ab35d-136">sendResponse</span></span>|<span data-ttu-id="ab35d-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab35d-137">Boolean</span></span>|<span data-ttu-id="ab35d-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="ab35d-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="ab35d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab35d-141">Response</span></span>

<span data-ttu-id="ab35d-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab35d-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab35d-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab35d-144">Example</span></span>
<span data-ttu-id="ab35d-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ab35d-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab35d-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab35d-146">Request</span></span>
<span data-ttu-id="ab35d-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab35d-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ab35d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab35d-148">Response</span></span>
##### <a name="response"></a><span data-ttu-id="ab35d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab35d-149">Response</span></span>
<span data-ttu-id="ab35d-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab35d-150">Here is an example of the response.</span></span>
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
