# <a name="create-calendar"></a><span data-ttu-id="3db8e-101">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="3db8e-101">Create Calendar</span></span>

<span data-ttu-id="3db8e-102">Use esta API para criar um novo calendário em um grupo de calendários para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="3db8e-102">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3db8e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="3db8e-103">Permissions</span></span>

<span data-ttu-id="3db8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3db8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="3db8e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3db8e-106">Permission type</span></span>                        | <span data-ttu-id="3db8e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3db8e-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3db8e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3db8e-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="3db8e-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db8e-109">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="3db8e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3db8e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3db8e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db8e-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="3db8e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3db8e-112">Application</span></span>                            | <span data-ttu-id="3db8e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db8e-113">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3db8e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3db8e-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3db8e-115">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="3db8e-115">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="3db8e-116">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3db8e-116">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="3db8e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3db8e-117">Request headers</span></span>

| <span data-ttu-id="3db8e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3db8e-118">Header</span></span>        | <span data-ttu-id="3db8e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="3db8e-119">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="3db8e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3db8e-120">Authorization</span></span> | <span data-ttu-id="3db8e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3db8e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3db8e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3db8e-123">Content-Type</span></span>  | <span data-ttu-id="3db8e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3db8e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3db8e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3db8e-126">Request body</span></span>

<span data-ttu-id="3db8e-127">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="3db8e-127">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3db8e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3db8e-128">Response</span></span>

<span data-ttu-id="3db8e-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3db8e-129">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3db8e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3db8e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3db8e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3db8e-131">Request</span></span>

<span data-ttu-id="3db8e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3db8e-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="3db8e-133">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="3db8e-133">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="3db8e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3db8e-134">Response</span></span>

<span data-ttu-id="3db8e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3db8e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
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
