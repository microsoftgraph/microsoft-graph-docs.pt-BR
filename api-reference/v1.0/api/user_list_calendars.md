# <a name="list-calendars"></a><span data-ttu-id="87140-101">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="87140-101">List calendars</span></span>

<span data-ttu-id="87140-102">Obtenha calendários de todos do usuário (propriedade de navegação `/calendars`), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico.</span><span class="sxs-lookup"><span data-stu-id="87140-102">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="87140-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87140-103">Prerequisites</span></span>
<span data-ttu-id="87140-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.Read; Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="87140-104">One of the following scopes is required to execute this API: Calendars.Read; Calendars.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="87140-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87140-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="87140-106">Calendários de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="87140-106">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="87140-107">Os calendários do usuário no [calendarGroup](../resources/calendarGroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="87140-107">The user's calendars in the default [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="87140-108">Os calendários do usuário em um [calendarGroup](../resources/calendarGroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="87140-108">The user's calendars in a specific [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87140-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87140-109">Optional query parameters</span></span>
<span data-ttu-id="87140-110">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87140-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87140-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87140-111">Request headers</span></span>
| <span data-ttu-id="87140-112">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87140-112">Header</span></span>       | <span data-ttu-id="87140-113">Valor</span><span class="sxs-lookup"><span data-stu-id="87140-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87140-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="87140-114">Authorization</span></span>  | <span data-ttu-id="87140-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87140-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="87140-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87140-117">Content-Type</span></span>   | <span data-ttu-id="87140-118">application/json</span><span class="sxs-lookup"><span data-stu-id="87140-118">application/json</span></span> | 

## <a name="request-body"></a><span data-ttu-id="87140-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87140-119">Request body</span></span>
<span data-ttu-id="87140-120">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87140-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87140-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="87140-121">Response</span></span>

<span data-ttu-id="87140-122">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87140-122">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87140-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87140-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87140-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87140-124">Request</span></span>
<span data-ttu-id="87140-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87140-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
##### <a name="response"></a><span data-ttu-id="87140-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="87140-126">Response</span></span>
<span data-ttu-id="87140-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87140-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars",
    "value": [
        {
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