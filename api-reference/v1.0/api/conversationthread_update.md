# <a name="update-conversationthread"></a><span data-ttu-id="d994a-101">Atualizar conversationthread</span><span class="sxs-lookup"><span data-stu-id="d994a-101">Update conversationthread</span></span>

<span data-ttu-id="d994a-102">Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.</span><span class="sxs-lookup"><span data-stu-id="d994a-102">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d994a-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d994a-103">Prerequisites</span></span>
<span data-ttu-id="d994a-104">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="d994a-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="d994a-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d994a-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d994a-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d994a-106">Request headers</span></span>
| <span data-ttu-id="d994a-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d994a-107">Header</span></span>       | <span data-ttu-id="d994a-108">Valor</span><span class="sxs-lookup"><span data-stu-id="d994a-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d994a-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="d994a-109">Authorization</span></span>  | <span data-ttu-id="d994a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d994a-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d994a-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d994a-112">Content-Type</span></span>  | <span data-ttu-id="d994a-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d994a-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d994a-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d994a-115">Request body</span></span>
<span data-ttu-id="d994a-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d994a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d994a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d994a-119">Property</span></span>     | <span data-ttu-id="d994a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d994a-120">Type</span></span>   |<span data-ttu-id="d994a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d994a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d994a-122">isLocked</span><span class="sxs-lookup"><span data-stu-id="d994a-122">isLocked</span></span>|<span data-ttu-id="d994a-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="d994a-123">Boolean</span></span>|<span data-ttu-id="d994a-p104">Indica se o thread está bloqueado. Defina como `true` para proibir a postagem.</span><span class="sxs-lookup"><span data-stu-id="d994a-p104">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="d994a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d994a-126">Response</span></span>

<span data-ttu-id="d994a-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d994a-127">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d994a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d994a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d994a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d994a-129">Request</span></span>
<span data-ttu-id="d994a-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d994a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="d994a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d994a-131">Response</span></span>
<span data-ttu-id="d994a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d994a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
