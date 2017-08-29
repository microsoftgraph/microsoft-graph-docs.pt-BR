# <a name="event-accept"></a><span data-ttu-id="b100f-101">event: accept</span><span class="sxs-lookup"><span data-stu-id="b100f-101">event: accept</span></span>

<span data-ttu-id="b100f-102">Aceita o evento especificado.</span><span class="sxs-lookup"><span data-stu-id="b100f-102">Accept the specified event.</span></span>

## <a name="permissions"></a><span data-ttu-id="b100f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b100f-103">Permissions</span></span>
<span data-ttu-id="b100f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b100f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b100f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b100f-106">Permission type</span></span>      | <span data-ttu-id="b100f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b100f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b100f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b100f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b100f-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b100f-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b100f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b100f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b100f-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b100f-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b100f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b100f-112">Application</span></span> | <span data-ttu-id="b100f-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b100f-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b100f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b100f-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="b100f-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b100f-115">Request headers</span></span>
| <span data-ttu-id="b100f-116">Nome</span><span class="sxs-lookup"><span data-stu-id="b100f-116">Name</span></span>       | <span data-ttu-id="b100f-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="b100f-117">Type</span></span> | <span data-ttu-id="b100f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="b100f-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b100f-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b100f-119">Authorization</span></span>  | <span data-ttu-id="b100f-120">string</span><span class="sxs-lookup"><span data-stu-id="b100f-120">string</span></span>  | <span data-ttu-id="b100f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b100f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b100f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b100f-123">Content-Type</span></span> | <span data-ttu-id="b100f-124">string</span><span class="sxs-lookup"><span data-stu-id="b100f-124">string</span></span>  | <span data-ttu-id="b100f-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b100f-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b100f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b100f-127">Request body</span></span>
<span data-ttu-id="b100f-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b100f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b100f-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b100f-129">Parameter</span></span>    | <span data-ttu-id="b100f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b100f-130">Type</span></span>   |<span data-ttu-id="b100f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b100f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b100f-132">comment</span><span class="sxs-lookup"><span data-stu-id="b100f-132">comment</span></span>|<span data-ttu-id="b100f-133">String</span><span class="sxs-lookup"><span data-stu-id="b100f-133">String</span></span>|<span data-ttu-id="b100f-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b100f-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="b100f-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="b100f-136">sendResponse</span></span>|<span data-ttu-id="b100f-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="b100f-137">Boolean</span></span>|<span data-ttu-id="b100f-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="b100f-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="b100f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b100f-141">Response</span></span>

<span data-ttu-id="b100f-p106">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b100f-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b100f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b100f-144">Example</span></span>
<span data-ttu-id="b100f-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b100f-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b100f-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b100f-146">Request</span></span>
<span data-ttu-id="b100f-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b100f-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b100f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b100f-148">Response</span></span>
<span data-ttu-id="b100f-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b100f-149">Here is an example of the response.</span></span>
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
