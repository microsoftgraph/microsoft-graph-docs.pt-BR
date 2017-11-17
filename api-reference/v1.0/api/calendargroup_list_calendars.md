# <a name="list-calendars"></a><span data-ttu-id="d8900-101">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="d8900-101">List calendars</span></span>

<span data-ttu-id="d8900-102">Recupera uma lista de calendários que pertencem a um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="d8900-102">Retrieve a list of calendars belonging to a calendar group.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8900-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8900-103">Permissions</span></span>
<span data-ttu-id="d8900-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8900-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d8900-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8900-106">Permission type</span></span>      | <span data-ttu-id="d8900-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8900-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8900-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8900-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d8900-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d8900-109">Calendars.Read</span></span>    |
|<span data-ttu-id="d8900-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8900-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8900-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d8900-111">Calendars.Read</span></span>    |
|<span data-ttu-id="d8900-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8900-112">Application</span></span> | <span data-ttu-id="d8900-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d8900-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8900-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8900-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d8900-115">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8900-115">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```
<span data-ttu-id="d8900-116">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d8900-116">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8900-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d8900-117">Optional query parameters</span></span>
<span data-ttu-id="d8900-118">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d8900-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8900-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8900-119">Request headers</span></span>
| <span data-ttu-id="d8900-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d8900-120">Name</span></span>       | <span data-ttu-id="d8900-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8900-121">Type</span></span> | <span data-ttu-id="d8900-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8900-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d8900-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8900-123">Authorization</span></span>  | <span data-ttu-id="d8900-124">string</span><span class="sxs-lookup"><span data-stu-id="d8900-124">string</span></span>  | <span data-ttu-id="d8900-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8900-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8900-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8900-127">Request body</span></span>
<span data-ttu-id="d8900-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8900-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8900-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8900-129">Response</span></span>

<span data-ttu-id="d8900-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8900-130">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8900-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8900-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8900-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8900-132">Request</span></span>
<span data-ttu-id="d8900-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8900-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```
##### <a name="response"></a><span data-ttu-id="d8900-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8900-134">Response</span></span>
<span data-ttu-id="d8900-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8900-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
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
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
