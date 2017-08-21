# <a name="create-event"></a><span data-ttu-id="1b6e3-101">Criar evento</span><span class="sxs-lookup"><span data-stu-id="1b6e3-101">Create Event</span></span>

<span data-ttu-id="1b6e3-102">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1b6e3-102">Use this API to create a new [event](../resources/event.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b6e3-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b6e3-103">Prerequisites</span></span>
<span data-ttu-id="1b6e3-104">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="1b6e3-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="1b6e3-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b6e3-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```
## <a name="request-headers"></a><span data-ttu-id="1b6e3-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6e3-106">Request headers</span></span>
| <span data-ttu-id="1b6e3-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b6e3-107">Header</span></span>       | <span data-ttu-id="1b6e3-108">Valor</span><span class="sxs-lookup"><span data-stu-id="1b6e3-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b6e3-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b6e3-109">Authorization</span></span>  | <span data-ttu-id="1b6e3-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b6e3-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b6e3-112">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6e3-112">Request body</span></span>
<span data-ttu-id="1b6e3-113">No corpo da solicitação, forneça uma representação JSON do objeto [Event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1b6e3-113">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1b6e3-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b6e3-114">Response</span></span>

<span data-ttu-id="1b6e3-115">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b6e3-115">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b6e3-116">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b6e3-116">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b6e3-117">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6e3-117">Request</span></span>
<span data-ttu-id="1b6e3-118">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b6e3-118">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="1b6e3-119">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1b6e3-119">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1b6e3-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b6e3-120">Response</span></span>
<span data-ttu-id="1b6e3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b6e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
