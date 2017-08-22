# <a name="create-calendargroup"></a><span data-ttu-id="cb985-101">Atualizar CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="cb985-101">Create CalendarGroup</span></span>

<span data-ttu-id="cb985-102">Use essa API para criar um novo CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="cb985-102">Use this API to create a new CalendarGroup.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb985-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cb985-103">Prerequisites</span></span>
<span data-ttu-id="cb985-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="cb985-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="cb985-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb985-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="cb985-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb985-106">Request headers</span></span>
| <span data-ttu-id="cb985-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb985-107">Header</span></span>       | <span data-ttu-id="cb985-108">Valor</span><span class="sxs-lookup"><span data-stu-id="cb985-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb985-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb985-109">Authorization</span></span>  | <span data-ttu-id="cb985-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb985-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cb985-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb985-112">Content-Type</span></span>  | <span data-ttu-id="cb985-113">application/json</span><span class="sxs-lookup"><span data-stu-id="cb985-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb985-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb985-114">Request body</span></span>
<span data-ttu-id="cb985-115">No corpo da solicitação, forneça uma representação JSON do objeto [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="cb985-115">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cb985-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb985-116">Response</span></span>

<span data-ttu-id="cb985-117">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb985-117">If successful, this method returns `201, Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb985-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb985-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb985-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb985-119">Request</span></span>
<span data-ttu-id="cb985-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb985-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="cb985-121">No corpo da solicitação, forneça uma representação JSON do objeto [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="cb985-121">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cb985-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb985-122">Response</span></span>
<span data-ttu-id="cb985-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb985-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
