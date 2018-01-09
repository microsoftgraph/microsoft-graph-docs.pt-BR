# <a name="create-event"></a><span data-ttu-id="a972d-101">Criar evento</span><span class="sxs-lookup"><span data-stu-id="a972d-101">Create Event</span></span>
<span data-ttu-id="a972d-102">Use esta API para criar um novo [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a972d-102">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a972d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a972d-103">Permissions</span></span>
<span data-ttu-id="a972d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a972d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a972d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a972d-106">Permission type</span></span>      | <span data-ttu-id="a972d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a972d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a972d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a972d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a972d-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a972d-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a972d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a972d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a972d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a972d-111">Not supported.</span></span>    |
|<span data-ttu-id="a972d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a972d-112">Application</span></span> | <span data-ttu-id="a972d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a972d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a972d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a972d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="a972d-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a972d-115">Request headers</span></span>
| <span data-ttu-id="a972d-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a972d-116">Header</span></span>       | <span data-ttu-id="a972d-117">Valor</span><span class="sxs-lookup"><span data-stu-id="a972d-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a972d-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="a972d-118">Authorization</span></span>  | <span data-ttu-id="a972d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a972d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a972d-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a972d-121">Request body</span></span>
<span data-ttu-id="a972d-122">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a972d-122">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a972d-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="a972d-123">Response</span></span>
<span data-ttu-id="a972d-124">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a972d-124">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a972d-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a972d-125">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a972d-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a972d-126">Request</span></span>
<span data-ttu-id="a972d-127">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a972d-127">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
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
<span data-ttu-id="a972d-128">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a972d-128">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="a972d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a972d-129">Response</span></span>
<span data-ttu-id="a972d-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a972d-130">Here is an example of the response.</span></span>
><span data-ttu-id="a972d-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a972d-131">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a972d-132">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a972d-132">All the properties will be returned from an actual call.</span></span>

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
