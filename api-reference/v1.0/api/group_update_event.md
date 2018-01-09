# <a name="update-event"></a><span data-ttu-id="8194a-101">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="8194a-101">Update event</span></span>
<span data-ttu-id="8194a-102">Atualize um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="8194a-102">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8194a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="8194a-103">Permissions</span></span>
<span data-ttu-id="8194a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8194a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8194a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8194a-106">Permission type</span></span>      | <span data-ttu-id="8194a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8194a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8194a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8194a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8194a-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8194a-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8194a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8194a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8194a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8194a-111">Not supported.</span></span>    |
|<span data-ttu-id="8194a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8194a-112">Application</span></span> | <span data-ttu-id="8194a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8194a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8194a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8194a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8194a-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8194a-115">Request headers</span></span>
| <span data-ttu-id="8194a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="8194a-116">Name</span></span>       | <span data-ttu-id="8194a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8194a-117">Type</span></span> | <span data-ttu-id="8194a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8194a-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8194a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="8194a-119">Authorization</span></span>  | <span data-ttu-id="8194a-120">string</span><span class="sxs-lookup"><span data-stu-id="8194a-120">string</span></span>  | <span data-ttu-id="8194a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8194a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8194a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8194a-123">Request body</span></span>
<span data-ttu-id="8194a-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8194a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="8194a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8194a-127">Response</span></span>
<span data-ttu-id="8194a-128">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8194a-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8194a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8194a-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8194a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8194a-130">Request</span></span>
<span data-ttu-id="8194a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8194a-131">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

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

#### <a name="response"></a><span data-ttu-id="8194a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8194a-132">Response</span></span>
<span data-ttu-id="8194a-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8194a-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->