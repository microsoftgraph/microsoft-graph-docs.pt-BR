# <a name="delete-event"></a><span data-ttu-id="91a4c-101">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="91a4c-101">Delete event</span></span>

<span data-ttu-id="91a4c-102">Exclua um evento.</span><span class="sxs-lookup"><span data-stu-id="91a4c-102">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="91a4c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="91a4c-103">Permissions</span></span>
<span data-ttu-id="91a4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="91a4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="91a4c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91a4c-106">Permission type</span></span>      | <span data-ttu-id="91a4c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91a4c-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="91a4c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91a4c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="91a4c-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91a4c-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="91a4c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91a4c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91a4c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91a4c-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="91a4c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91a4c-112">Application</span></span> | <span data-ttu-id="91a4c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91a4c-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="91a4c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91a4c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="91a4c-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91a4c-115">Request headers</span></span>
| <span data-ttu-id="91a4c-116">Nome</span><span class="sxs-lookup"><span data-stu-id="91a4c-116">Name</span></span>       | <span data-ttu-id="91a4c-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="91a4c-117">Type</span></span> | <span data-ttu-id="91a4c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="91a4c-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91a4c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="91a4c-119">Authorization</span></span>  | <span data-ttu-id="91a4c-120">string</span><span class="sxs-lookup"><span data-stu-id="91a4c-120">string</span></span>  | <span data-ttu-id="91a4c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91a4c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91a4c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91a4c-123">Request body</span></span>
<span data-ttu-id="91a4c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91a4c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91a4c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="91a4c-125">Response</span></span>

<span data-ttu-id="91a4c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91a4c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91a4c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91a4c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91a4c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91a4c-129">Request</span></span>
<span data-ttu-id="91a4c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91a4c-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="91a4c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="91a4c-131">Response</span></span>
<span data-ttu-id="91a4c-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91a4c-132">Here is an example of the response.</span></span> 
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
