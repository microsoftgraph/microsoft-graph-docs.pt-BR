# <a name="create-calendar"></a><span data-ttu-id="7be39-101">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="7be39-101">Create Calendar</span></span>

<span data-ttu-id="7be39-102">Use esta API para criar um novo calendário.</span><span class="sxs-lookup"><span data-stu-id="7be39-102">Use this API to create a new calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="7be39-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7be39-103">Permissions</span></span>
<span data-ttu-id="7be39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7be39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7be39-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7be39-106">Permission type</span></span>      | <span data-ttu-id="7be39-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7be39-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7be39-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7be39-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7be39-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7be39-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7be39-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7be39-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7be39-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7be39-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7be39-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7be39-112">Application</span></span> | <span data-ttu-id="7be39-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7be39-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7be39-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7be39-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="7be39-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7be39-115">Request headers</span></span>
| <span data-ttu-id="7be39-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7be39-116">Header</span></span>       | <span data-ttu-id="7be39-117">Valor</span><span class="sxs-lookup"><span data-stu-id="7be39-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7be39-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="7be39-118">Authorization</span></span>  | <span data-ttu-id="7be39-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7be39-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7be39-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7be39-121">Content-Type</span></span>  | <span data-ttu-id="7be39-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7be39-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7be39-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7be39-123">Request body</span></span>
<span data-ttu-id="7be39-124">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="7be39-124">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7be39-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7be39-125">Response</span></span>

<span data-ttu-id="7be39-126">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7be39-126">If successful, this method returns `201, Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7be39-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7be39-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7be39-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7be39-128">Request</span></span>
<span data-ttu-id="7be39-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7be39-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="7be39-130">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="7be39-130">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7be39-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7be39-131">Response</span></span>
<span data-ttu-id="7be39-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7be39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
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
