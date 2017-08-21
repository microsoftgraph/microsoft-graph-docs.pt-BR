# <a name="create-calendar"></a><span data-ttu-id="e26e4-101">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="e26e4-101">Create Calendar</span></span>

<span data-ttu-id="e26e4-102">Use esta API para criar um novo calendário.</span><span class="sxs-lookup"><span data-stu-id="e26e4-102">Use this API to create a new calendar.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e26e4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e26e4-103">Prerequisites</span></span>
<span data-ttu-id="e26e4-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="e26e4-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="e26e4-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e26e4-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="e26e4-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e26e4-106">Request headers</span></span>
| <span data-ttu-id="e26e4-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e26e4-107">Header</span></span>       | <span data-ttu-id="e26e4-108">Valor</span><span class="sxs-lookup"><span data-stu-id="e26e4-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e26e4-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="e26e4-109">Authorization</span></span>  | <span data-ttu-id="e26e4-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e26e4-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e26e4-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e26e4-112">Content-Type</span></span>  | <span data-ttu-id="e26e4-113">application/json</span><span class="sxs-lookup"><span data-stu-id="e26e4-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e26e4-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e26e4-114">Request body</span></span>
<span data-ttu-id="e26e4-115">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="e26e4-115">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e26e4-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="e26e4-116">Response</span></span>

<span data-ttu-id="e26e4-117">Se for bem sucedido, esse método retornará um código de resposta `201, Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e26e4-117">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e26e4-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e26e4-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e26e4-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e26e4-119">Request</span></span>
<span data-ttu-id="e26e4-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e26e4-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="e26e4-121">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="e26e4-121">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e26e4-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="e26e4-122">Response</span></span>
<span data-ttu-id="e26e4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e26e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "canEdit":true,
    "owner":{
        "name":"Fanny Downs",
        "address":"fannyd@adatum.onmicrosoft.com"
    }
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
