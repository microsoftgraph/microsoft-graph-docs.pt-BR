# <a name="delete-calendar"></a><span data-ttu-id="7484a-101">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="7484a-101">Delete calendar</span></span>

<span data-ttu-id="7484a-102">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="7484a-102">Delete a calendar other than the default calendar.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7484a-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7484a-103">Prerequisites</span></span>
<span data-ttu-id="7484a-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="7484a-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="7484a-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7484a-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="7484a-106">Um [calendar](../resources/calendar.md) de usuário, que não seja o padrão, no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="7484a-106">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="7484a-107">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="7484a-107">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7484a-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7484a-108">Request headers</span></span>
| <span data-ttu-id="7484a-109">Nome</span><span class="sxs-lookup"><span data-stu-id="7484a-109">Name</span></span>           |  <span data-ttu-id="7484a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7484a-110">Type</span></span>    | <span data-ttu-id="7484a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7484a-111">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="7484a-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="7484a-112">Authorization</span></span>  |  <span data-ttu-id="7484a-113">string</span><span class="sxs-lookup"><span data-stu-id="7484a-113">string</span></span>  | <span data-ttu-id="7484a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7484a-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7484a-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7484a-116">Request body</span></span>
<span data-ttu-id="7484a-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7484a-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7484a-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="7484a-118">Response</span></span>

<span data-ttu-id="7484a-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7484a-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7484a-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7484a-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7484a-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7484a-122">Request</span></span>
<span data-ttu-id="7484a-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7484a-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="7484a-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="7484a-124">Response</span></span>
<span data-ttu-id="7484a-125">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7484a-125">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
