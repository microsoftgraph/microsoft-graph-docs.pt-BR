# <a name="delete-calendar"></a><span data-ttu-id="13389-101">Excluir calendário</span><span class="sxs-lookup"><span data-stu-id="13389-101">Delete calendar</span></span>

<span data-ttu-id="13389-102">Exclua um calendário que não o calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="13389-102">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="13389-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="13389-103">Permissions</span></span>
<span data-ttu-id="13389-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="13389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="13389-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13389-106">Permission type</span></span>      | <span data-ttu-id="13389-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13389-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="13389-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13389-108">Delegated (work or school account)</span></span> | <span data-ttu-id="13389-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13389-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="13389-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13389-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13389-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13389-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="13389-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13389-112">Application</span></span> | <span data-ttu-id="13389-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13389-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="13389-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13389-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="13389-115">Um [calendar](../resources/calendar.md) de usuário, que não seja o padrão, no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="13389-115">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="13389-116">Um [calendar](../resources/calendar.md), que não seja o padrão, em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="13389-116">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="13389-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13389-117">Request headers</span></span>
| <span data-ttu-id="13389-118">Nome</span><span class="sxs-lookup"><span data-stu-id="13389-118">Name</span></span>           |  <span data-ttu-id="13389-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="13389-119">Type</span></span>    | <span data-ttu-id="13389-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="13389-120">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="13389-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13389-121">Authorization</span></span>  |  <span data-ttu-id="13389-122">string</span><span class="sxs-lookup"><span data-stu-id="13389-122">string</span></span>  | <span data-ttu-id="13389-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13389-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13389-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13389-125">Request body</span></span>
<span data-ttu-id="13389-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13389-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13389-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="13389-127">Response</span></span>

<span data-ttu-id="13389-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13389-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13389-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13389-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13389-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13389-131">Request</span></span>
<span data-ttu-id="13389-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13389-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="13389-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="13389-133">Response</span></span>
<span data-ttu-id="13389-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13389-134">Here is an example of the response.</span></span> 
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
