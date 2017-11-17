# <a name="create-event"></a><span data-ttu-id="07dd3-101">Criar evento</span><span class="sxs-lookup"><span data-stu-id="07dd3-101">Create Event</span></span>

<span data-ttu-id="07dd3-102">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="07dd3-102">Use this API to create a new [event](../resources/event.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="07dd3-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="07dd3-103">Permissions</span></span>
<span data-ttu-id="07dd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="07dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="07dd3-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07dd3-106">Permission type</span></span>      | <span data-ttu-id="07dd3-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07dd3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07dd3-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07dd3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="07dd3-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07dd3-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="07dd3-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07dd3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07dd3-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07dd3-111">Not supported.</span></span>    |
|<span data-ttu-id="07dd3-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07dd3-112">Application</span></span> | <span data-ttu-id="07dd3-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07dd3-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07dd3-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07dd3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```
## <a name="request-headers"></a><span data-ttu-id="07dd3-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07dd3-115">Request headers</span></span>
| <span data-ttu-id="07dd3-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07dd3-116">Header</span></span>       | <span data-ttu-id="07dd3-117">Valor</span><span class="sxs-lookup"><span data-stu-id="07dd3-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07dd3-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="07dd3-118">Authorization</span></span>  | <span data-ttu-id="07dd3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07dd3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07dd3-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07dd3-121">Request body</span></span>
<span data-ttu-id="07dd3-122">No corpo da solicitação, forneça uma representação JSON do objeto [Event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="07dd3-122">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="07dd3-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="07dd3-123">Response</span></span>

<span data-ttu-id="07dd3-124">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07dd3-124">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07dd3-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07dd3-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07dd3-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07dd3-126">Request</span></span>
<span data-ttu-id="07dd3-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07dd3-127">Here is an example of the request.</span></span>
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
<span data-ttu-id="07dd3-128">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="07dd3-128">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="07dd3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="07dd3-129">Response</span></span>
<span data-ttu-id="07dd3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07dd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
