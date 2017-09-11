# <a name="list-calendars"></a><span data-ttu-id="6c833-101">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="6c833-101">List calendars</span></span>

<span data-ttu-id="6c833-102">Obtenha calendários de todos do usuário (propriedade de navegação `/calendars`), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico.</span><span class="sxs-lookup"><span data-stu-id="6c833-102">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="6c833-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c833-103">Permissions</span></span>
<span data-ttu-id="6c833-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6c833-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c833-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c833-106">Permission type</span></span>      | <span data-ttu-id="6c833-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c833-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c833-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c833-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6c833-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c833-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6c833-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c833-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c833-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c833-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6c833-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c833-112">Application</span></span> | <span data-ttu-id="6c833-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c833-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c833-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c833-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="6c833-115">Calendários de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="6c833-115">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="6c833-116">Os calendários do usuário no [calendarGroup](../resources/calendarGroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="6c833-116">The user's calendars in the default [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="6c833-117">Os calendários do usuário em um [calendarGroup](../resources/calendarGroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="6c833-117">The user's calendars in a specific [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c833-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c833-118">Optional query parameters</span></span>
<span data-ttu-id="6c833-119">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6c833-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6c833-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c833-120">Request headers</span></span>
| <span data-ttu-id="6c833-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c833-121">Header</span></span>       | <span data-ttu-id="6c833-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6c833-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c833-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c833-123">Authorization</span></span>  | <span data-ttu-id="6c833-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c833-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6c833-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c833-126">Content-Type</span></span>   | <span data-ttu-id="6c833-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c833-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c833-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c833-128">Request body</span></span>
<span data-ttu-id="6c833-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c833-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c833-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c833-130">Response</span></span>

<span data-ttu-id="6c833-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c833-131">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c833-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c833-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c833-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c833-133">Request</span></span>
<span data-ttu-id="6c833-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c833-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
##### <a name="response"></a><span data-ttu-id="6c833-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c833-135">Response</span></span>
<span data-ttu-id="6c833-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c833-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
                "name":"Samantha Booth",
                "address":"samanthab@adatum.onmicrosoft.com"
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