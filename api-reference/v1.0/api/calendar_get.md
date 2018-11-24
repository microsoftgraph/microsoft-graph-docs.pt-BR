# <a name="get-calendar"></a><span data-ttu-id="0d401-101">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="0d401-101">Get calendar</span></span>

<span data-ttu-id="0d401-102">Obtenha as propriedades e as relações de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="0d401-102">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="0d401-103">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="0d401-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="0d401-104">Há dois cenários onde um aplicativo pode obter o calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="0d401-104">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="0d401-105">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="0d401-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0d401-106">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou um calendário com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="0d401-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0d401-107">Consulte os [detalhes e um exemplo](../../../concepts/outlook-get-shared-events-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="0d401-107">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d401-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="0d401-108">Permissions</span></span>
<span data-ttu-id="0d401-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d401-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0d401-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d401-111">Permission type</span></span>      | <span data-ttu-id="0d401-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d401-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d401-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d401-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0d401-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0d401-114">Calendars.Read</span></span>    |
|<span data-ttu-id="0d401-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d401-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d401-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0d401-116">Calendars.Read</span></span>    |
|<span data-ttu-id="0d401-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d401-117">Application</span></span> | <span data-ttu-id="0d401-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0d401-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d401-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d401-119">HTTP request</span></span>
<span data-ttu-id="0d401-120"><!-- { "blockType": "ignored" } -->Um usuário ou do grupo padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="0d401-120"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="0d401-121">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="0d401-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="0d401-122">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="0d401-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d401-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0d401-123">Optional query parameters</span></span>
<span data-ttu-id="0d401-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d401-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0d401-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d401-125">Request headers</span></span>
| <span data-ttu-id="0d401-126">Nome</span><span class="sxs-lookup"><span data-stu-id="0d401-126">Name</span></span>       | <span data-ttu-id="0d401-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d401-127">Type</span></span> | <span data-ttu-id="0d401-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d401-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0d401-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d401-129">Authorization</span></span>  | <span data-ttu-id="0d401-130">string</span><span class="sxs-lookup"><span data-stu-id="0d401-130">string</span></span>  | <span data-ttu-id="0d401-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d401-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d401-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d401-133">Request body</span></span>
<span data-ttu-id="0d401-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d401-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d401-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d401-135">Response</span></span>

<span data-ttu-id="0d401-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d401-136">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d401-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d401-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d401-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d401-138">Request</span></span>
<span data-ttu-id="0d401-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d401-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="0d401-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d401-140">Response</span></span>
<span data-ttu-id="0d401-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d401-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
