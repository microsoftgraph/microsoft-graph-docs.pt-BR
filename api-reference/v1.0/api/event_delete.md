# <a name="delete-event"></a><span data-ttu-id="56ca6-101">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="56ca6-101">Delete event</span></span>

<span data-ttu-id="56ca6-102">Exclui um evento.</span><span class="sxs-lookup"><span data-stu-id="56ca6-102">Delete event.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56ca6-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56ca6-103">Prerequisites</span></span>
<span data-ttu-id="56ca6-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="56ca6-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span> 
## <a name="http-request"></a><span data-ttu-id="56ca6-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56ca6-105">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="56ca6-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56ca6-106">Request headers</span></span>
| <span data-ttu-id="56ca6-107">Nome</span><span class="sxs-lookup"><span data-stu-id="56ca6-107">Name</span></span>       | <span data-ttu-id="56ca6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="56ca6-108">Type</span></span> | <span data-ttu-id="56ca6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ca6-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="56ca6-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="56ca6-110">Authorization</span></span>  | <span data-ttu-id="56ca6-111">string</span><span class="sxs-lookup"><span data-stu-id="56ca6-111">string</span></span>  | <span data-ttu-id="56ca6-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56ca6-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56ca6-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56ca6-114">Request body</span></span>
<span data-ttu-id="56ca6-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56ca6-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56ca6-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ca6-116">Response</span></span>

<span data-ttu-id="56ca6-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56ca6-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56ca6-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56ca6-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56ca6-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56ca6-120">Request</span></span>
<span data-ttu-id="56ca6-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56ca6-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="56ca6-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ca6-122">Response</span></span>
<span data-ttu-id="56ca6-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56ca6-123">Here is an example of the response.</span></span> 
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
