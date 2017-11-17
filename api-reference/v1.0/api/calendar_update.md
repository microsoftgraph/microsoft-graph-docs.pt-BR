# <a name="update-calendar"></a><span data-ttu-id="3de8e-101">Atualizar o calendário</span><span class="sxs-lookup"><span data-stu-id="3de8e-101">Update calendar</span></span>

<span data-ttu-id="3de8e-102">Atualize as propriedades de um objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="3de8e-102">Update the properties of calendar object.</span></span> <span data-ttu-id="3de8e-103">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3de8e-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3de8e-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="3de8e-104">Permissions</span></span>
<span data-ttu-id="3de8e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3de8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3de8e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3de8e-107">Permission type</span></span>      | <span data-ttu-id="3de8e-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3de8e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3de8e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3de8e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3de8e-110">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3de8e-110">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3de8e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3de8e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3de8e-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3de8e-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3de8e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3de8e-113">Application</span></span> | <span data-ttu-id="3de8e-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3de8e-114">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3de8e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3de8e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="3de8e-116">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="3de8e-116">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="3de8e-117">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="3de8e-117">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="3de8e-118">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="3de8e-118">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3de8e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3de8e-119">Request headers</span></span>
| <span data-ttu-id="3de8e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3de8e-120">Header</span></span>       | <span data-ttu-id="3de8e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3de8e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3de8e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3de8e-122">Authorization</span></span>  | <span data-ttu-id="3de8e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3de8e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3de8e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3de8e-125">Content-Type</span></span>  | <span data-ttu-id="3de8e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3de8e-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3de8e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3de8e-128">Request body</span></span>
<span data-ttu-id="3de8e-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3de8e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3de8e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3de8e-132">Property</span></span>     | <span data-ttu-id="3de8e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3de8e-133">Type</span></span>   |<span data-ttu-id="3de8e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3de8e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3de8e-135">color</span><span class="sxs-lookup"><span data-stu-id="3de8e-135">color</span></span>|<span data-ttu-id="3de8e-136">String</span><span class="sxs-lookup"><span data-stu-id="3de8e-136">String</span></span>|<span data-ttu-id="3de8e-p106">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="3de8e-p106">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="3de8e-139">nome</span><span class="sxs-lookup"><span data-stu-id="3de8e-139">name</span></span>|<span data-ttu-id="3de8e-140">String</span><span class="sxs-lookup"><span data-stu-id="3de8e-140">String</span></span>|<span data-ttu-id="3de8e-141">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="3de8e-141">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="3de8e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3de8e-142">Response</span></span>

<span data-ttu-id="3de8e-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3de8e-143">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3de8e-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3de8e-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3de8e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3de8e-145">Request</span></span>
<span data-ttu-id="3de8e-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3de8e-146">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3de8e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="3de8e-147">Response</span></span>
<span data-ttu-id="3de8e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3de8e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
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
