# <a name="get-calendar"></a><span data-ttu-id="7d429-101">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="7d429-101">Get calendar</span></span>

<span data-ttu-id="7d429-102">Recuperar as propriedades e os relacionamentos do objeto calendar.</span><span class="sxs-lookup"><span data-stu-id="7d429-102">Retrieve the properties and relationships of calendar object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d429-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d429-103">Permissions</span></span>
<span data-ttu-id="7d429-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7d429-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d429-106">Permission type</span></span>      | <span data-ttu-id="7d429-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d429-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d429-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d429-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7d429-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7d429-109">Calendars.Read</span></span>    |
|<span data-ttu-id="7d429-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d429-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d429-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7d429-111">Calendars.Read</span></span>    |
|<span data-ttu-id="7d429-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d429-112">Application</span></span> | <span data-ttu-id="7d429-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7d429-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d429-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d429-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="7d429-115">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="7d429-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="7d429-116">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="7d429-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="7d429-117">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="7d429-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d429-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d429-118">Optional query parameters</span></span>
<span data-ttu-id="7d429-119">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d429-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7d429-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d429-120">Request headers</span></span>
| <span data-ttu-id="7d429-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7d429-121">Name</span></span>       | <span data-ttu-id="7d429-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d429-122">Type</span></span> | <span data-ttu-id="7d429-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d429-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7d429-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d429-124">Authorization</span></span>  | <span data-ttu-id="7d429-125">string</span><span class="sxs-lookup"><span data-stu-id="7d429-125">string</span></span>  | <span data-ttu-id="7d429-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d429-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d429-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d429-128">Request body</span></span>
<span data-ttu-id="7d429-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d429-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d429-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d429-130">Response</span></span>

<span data-ttu-id="7d429-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d429-131">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d429-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d429-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d429-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d429-133">Request</span></span>
<span data-ttu-id="7d429-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d429-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="7d429-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d429-135">Response</span></span>
<span data-ttu-id="7d429-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d429-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
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
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
