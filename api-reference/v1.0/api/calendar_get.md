# <a name="get-calendar"></a><span data-ttu-id="7bba7-101">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="7bba7-101">Get calendar</span></span>

<span data-ttu-id="7bba7-102">Recuperar as propriedades e os relacionamentos do objeto calendar.</span><span class="sxs-lookup"><span data-stu-id="7bba7-102">Retrieve the properties and relationships of calendar object.</span></span>


### <a name="get-another-users-calendar"></a><span data-ttu-id="7bba7-103">Obter o calendário de outro usuário</span><span class="sxs-lookup"><span data-stu-id="7bba7-103">Get another user's drive</span></span>

<span data-ttu-id="7bba7-104">Se você tiver permissões de aplicativo ou se tiver as [permissões](#permissions) delegadas apropriadas de um usuário, será possível obter o calendário de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="7bba7-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get a calendar of another user's.</span></span> <span data-ttu-id="7bba7-105">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="7bba7-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="7bba7-106">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="7bba7-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="7bba7-107">Suponha que outro usuário, Henrique, tenha um calendário compartilhado com Diogo.</span><span class="sxs-lookup"><span data-stu-id="7bba7-107">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="7bba7-108">Você pode obter esse calendário compartilhado especificando a ID de usuário de Henrique (ou nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="7bba7-108">You can get that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="7bba7-109">Esse recurso se aplica a todas as operações de calendário GET com suporte para usuários individuais, conforme listado na seção [Solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="7bba7-109">This capability applies to all the supported GET calendar operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="7bba7-110">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="7bba7-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="7bba7-111">Se Henrique não tiver compartilhado seu calendário com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="7bba7-111">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="7bba7-112">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para obter o calendário do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="7bba7-112">In such cases, specifying a user ID or user principal name only works for getting a calendar of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar
```

<span data-ttu-id="7bba7-113">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="7bba7-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="7bba7-114">Pastas de contatos compartilhadas</span><span class="sxs-lookup"><span data-stu-id="7bba7-114">Shared contact folders</span></span>
- <span data-ttu-id="7bba7-115">Calendários compartilhados</span><span class="sxs-lookup"><span data-stu-id="7bba7-115">Shared calendars</span></span>
- <span data-ttu-id="7bba7-116">Contatos e eventos em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="7bba7-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="7bba7-117">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="7bba7-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="7bba7-118">Esse recurso não está disponível em outras operações para contatos, eventos e suas pastas.</span><span class="sxs-lookup"><span data-stu-id="7bba7-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="7bba7-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bba7-119">Permissions</span></span>
<span data-ttu-id="7bba7-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bba7-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7bba7-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bba7-122">Permission type</span></span>      | <span data-ttu-id="7bba7-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bba7-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bba7-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bba7-124">Delegated (work or school account)</span></span> | <span data-ttu-id="7bba7-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7bba7-125">Calendars.Read</span></span>    |
|<span data-ttu-id="7bba7-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bba7-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bba7-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7bba7-127">Calendars.Read</span></span>    |
|<span data-ttu-id="7bba7-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bba7-128">Application</span></span> | <span data-ttu-id="7bba7-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7bba7-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bba7-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bba7-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="7bba7-131">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="7bba7-131">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="7bba7-132">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="7bba7-132">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="7bba7-133">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="7bba7-133">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7bba7-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7bba7-134">Optional query parameters</span></span>
<span data-ttu-id="7bba7-135">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7bba7-135">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7bba7-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bba7-136">Request headers</span></span>
| <span data-ttu-id="7bba7-137">Nome</span><span class="sxs-lookup"><span data-stu-id="7bba7-137">Name</span></span>       | <span data-ttu-id="7bba7-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bba7-138">Type</span></span> | <span data-ttu-id="7bba7-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bba7-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7bba7-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bba7-140">Authorization</span></span>  | <span data-ttu-id="7bba7-141">string</span><span class="sxs-lookup"><span data-stu-id="7bba7-141">string</span></span>  | <span data-ttu-id="7bba7-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bba7-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bba7-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bba7-144">Request body</span></span>
<span data-ttu-id="7bba7-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bba7-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bba7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bba7-146">Response</span></span>

<span data-ttu-id="7bba7-147">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bba7-147">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bba7-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bba7-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bba7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bba7-149">Request</span></span>
<span data-ttu-id="7bba7-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bba7-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="7bba7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bba7-151">Response</span></span>
<span data-ttu-id="7bba7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bba7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
