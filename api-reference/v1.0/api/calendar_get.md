# <a name="get-calendar"></a><span data-ttu-id="b249b-101">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="b249b-101">Get calendar</span></span>

<span data-ttu-id="b249b-102">Recupera as propriedades e os relacionamentos do objeto de calendário.</span><span class="sxs-lookup"><span data-stu-id="b249b-102">Retrieve the properties and relationships of calendar object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b249b-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b249b-103">Prerequisites</span></span>
<span data-ttu-id="b249b-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.Read*</span><span class="sxs-lookup"><span data-stu-id="b249b-104">One of the following **scopes** is required to execute this API: *Calendars.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="b249b-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b249b-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b249b-106">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="b249b-106">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="b249b-107">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="b249b-107">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="b249b-108">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="b249b-108">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b249b-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b249b-109">Optional query parameters</span></span>
<span data-ttu-id="b249b-110">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b249b-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b249b-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b249b-111">Request headers</span></span>
| <span data-ttu-id="b249b-112">Nome</span><span class="sxs-lookup"><span data-stu-id="b249b-112">Name</span></span>       | <span data-ttu-id="b249b-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b249b-113">Type</span></span> | <span data-ttu-id="b249b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b249b-114">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b249b-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="b249b-115">Authorization</span></span>  | <span data-ttu-id="b249b-116">string</span><span class="sxs-lookup"><span data-stu-id="b249b-116">string</span></span>  | <span data-ttu-id="b249b-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b249b-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b249b-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b249b-119">Request body</span></span>
<span data-ttu-id="b249b-120">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b249b-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b249b-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="b249b-121">Response</span></span>

<span data-ttu-id="b249b-122">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b249b-122">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b249b-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b249b-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b249b-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b249b-124">Request</span></span>
<span data-ttu-id="b249b-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b249b-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="b249b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b249b-126">Response</span></span>
<span data-ttu-id="b249b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b249b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name":"Fanny Downs",
        "address":"fannyd@adatum.onmicrosoft.com"
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
