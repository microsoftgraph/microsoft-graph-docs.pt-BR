# <a name="create-calendargroup"></a><span data-ttu-id="05afc-101">Atualizar CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="05afc-101">Create CalendarGroup</span></span>

<span data-ttu-id="05afc-102">Use esta API para criar um novo CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="05afc-102">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="05afc-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="05afc-103">Permissions</span></span>
<span data-ttu-id="05afc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="05afc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="05afc-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05afc-106">Permission type</span></span>      | <span data-ttu-id="05afc-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05afc-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="05afc-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05afc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="05afc-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05afc-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="05afc-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05afc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05afc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05afc-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="05afc-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05afc-112">Application</span></span> | <span data-ttu-id="05afc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05afc-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="05afc-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05afc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="05afc-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05afc-115">Request headers</span></span>
| <span data-ttu-id="05afc-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05afc-116">Header</span></span>       | <span data-ttu-id="05afc-117">Valor</span><span class="sxs-lookup"><span data-stu-id="05afc-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05afc-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="05afc-118">Authorization</span></span>  | <span data-ttu-id="05afc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05afc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="05afc-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05afc-121">Content-Type</span></span>  | <span data-ttu-id="05afc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="05afc-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="05afc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05afc-123">Request body</span></span>
<span data-ttu-id="05afc-124">No corpo da solicitação, forneça uma representação JSON do objeto [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="05afc-124">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="05afc-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="05afc-125">Response</span></span>

<span data-ttu-id="05afc-126">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05afc-126">If successful, this method returns `201, Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05afc-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05afc-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05afc-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05afc-128">Request</span></span>
<span data-ttu-id="05afc-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05afc-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="05afc-130">No corpo da solicitação, forneça uma representação JSON do objeto [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="05afc-130">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="05afc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="05afc-131">Response</span></span>
<span data-ttu-id="05afc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05afc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
