# <a name="list-calendargroups"></a><span data-ttu-id="65797-101">Listar CalendarGroups</span><span class="sxs-lookup"><span data-stu-id="65797-101">List calendarGroups</span></span>

<span data-ttu-id="65797-102">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="65797-102">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="65797-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="65797-103">Permissions</span></span>
<span data-ttu-id="65797-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65797-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65797-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65797-106">Permission type</span></span>      | <span data-ttu-id="65797-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65797-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="65797-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65797-108">Delegated (work or school account)</span></span> | <span data-ttu-id="65797-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65797-109">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="65797-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65797-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65797-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65797-111">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="65797-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65797-112">Application</span></span> | <span data-ttu-id="65797-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65797-113">Calendars.Read, Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="65797-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65797-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65797-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65797-115">Optional query parameters</span></span>
<span data-ttu-id="65797-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65797-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="65797-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65797-117">Request headers</span></span>
| <span data-ttu-id="65797-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65797-118">Header</span></span>       | <span data-ttu-id="65797-119">Valor</span><span class="sxs-lookup"><span data-stu-id="65797-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="65797-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="65797-120">Authorization</span></span>  | <span data-ttu-id="65797-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65797-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="65797-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65797-123">Content-Type</span></span>  | <span data-ttu-id="65797-124">application/json</span><span class="sxs-lookup"><span data-stu-id="65797-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65797-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65797-125">Request body</span></span>
<span data-ttu-id="65797-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65797-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65797-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="65797-127">Response</span></span>

<span data-ttu-id="65797-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65797-128">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65797-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65797-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65797-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65797-130">Request</span></span>
<span data-ttu-id="65797-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65797-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="65797-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="65797-132">Response</span></span>
<span data-ttu-id="65797-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65797-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "name": "name-value",
      "classId": "classId-value",
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
