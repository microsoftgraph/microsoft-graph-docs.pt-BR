# <a name="update-calendar"></a><span data-ttu-id="89d34-101">Atualizar calendário</span><span class="sxs-lookup"><span data-stu-id="89d34-101">Update calendar</span></span>

<span data-ttu-id="89d34-102">Atualize as propriedades do objeto calendar.</span><span class="sxs-lookup"><span data-stu-id="89d34-102">Update the properties of calendar object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89d34-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89d34-103">Prerequisites</span></span>
<span data-ttu-id="89d34-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="89d34-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="89d34-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89d34-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="89d34-106">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="89d34-106">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="89d34-107">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="89d34-107">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="89d34-108">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="89d34-108">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="89d34-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89d34-109">Request headers</span></span>
| <span data-ttu-id="89d34-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89d34-110">Header</span></span>       | <span data-ttu-id="89d34-111">Valor</span><span class="sxs-lookup"><span data-stu-id="89d34-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89d34-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="89d34-112">Authorization</span></span>  | <span data-ttu-id="89d34-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89d34-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="89d34-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89d34-115">Content-Type</span></span>  | <span data-ttu-id="89d34-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89d34-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89d34-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89d34-118">Request body</span></span>
<span data-ttu-id="89d34-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="89d34-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="89d34-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89d34-122">Property</span></span>     | <span data-ttu-id="89d34-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="89d34-123">Type</span></span>   |<span data-ttu-id="89d34-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="89d34-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89d34-125">color</span><span class="sxs-lookup"><span data-stu-id="89d34-125">color</span></span>|<span data-ttu-id="89d34-126">String</span><span class="sxs-lookup"><span data-stu-id="89d34-126">String</span></span>|<span data-ttu-id="89d34-p104">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="89d34-p104">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="89d34-129">nome</span><span class="sxs-lookup"><span data-stu-id="89d34-129">name</span></span>|<span data-ttu-id="89d34-130">String</span><span class="sxs-lookup"><span data-stu-id="89d34-130">String</span></span>|<span data-ttu-id="89d34-131">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="89d34-131">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="89d34-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="89d34-132">Response</span></span>

<span data-ttu-id="89d34-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89d34-133">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89d34-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89d34-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89d34-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89d34-135">Request</span></span>
<span data-ttu-id="89d34-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89d34-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
##### <a name="response"></a><span data-ttu-id="89d34-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="89d34-137">Response</span></span>
<span data-ttu-id="89d34-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89d34-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
