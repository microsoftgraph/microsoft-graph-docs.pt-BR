# <a name="create-calendar"></a><span data-ttu-id="921b0-101">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="921b0-101">Create Calendar</span></span>

<span data-ttu-id="921b0-102">Use esta API para criar um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="921b0-102">Use this API to create a new Calendar in a calendar group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="921b0-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="921b0-103">Prerequisites</span></span>
<span data-ttu-id="921b0-104">Um dos seguintes **escopos** é necessário para executar esta API: _Calendars.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="921b0-104">One of the following **scopes** is required to execute this API: _Calendars.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="921b0-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="921b0-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="921b0-106">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="921b0-106">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```
<span data-ttu-id="921b0-107">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="921b0-107">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="921b0-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="921b0-108">Request headers</span></span>
| <span data-ttu-id="921b0-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="921b0-109">Header</span></span>       | <span data-ttu-id="921b0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="921b0-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="921b0-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="921b0-111">Authorization</span></span>  | <span data-ttu-id="921b0-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="921b0-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="921b0-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="921b0-114">Content-Type</span></span>  | <span data-ttu-id="921b0-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="921b0-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="921b0-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="921b0-117">Request body</span></span>
<span data-ttu-id="921b0-118">No corpo da solicitação, forneça uma representação JSON do objeto [Calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="921b0-118">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="921b0-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="921b0-119">Response</span></span>

<span data-ttu-id="921b0-120">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="921b0-120">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="921b0-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="921b0-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="921b0-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="921b0-122">Request</span></span>
<span data-ttu-id="921b0-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="921b0-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```
<span data-ttu-id="921b0-124">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="921b0-124">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="921b0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="921b0-125">Response</span></span>
<span data-ttu-id="921b0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="921b0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
