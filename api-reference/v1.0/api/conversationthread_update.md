# <a name="update-conversationthread"></a><span data-ttu-id="faf34-101">Atualizar conversationthread</span><span class="sxs-lookup"><span data-stu-id="faf34-101">Update conversationthread</span></span>

<span data-ttu-id="faf34-102">Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.</span><span class="sxs-lookup"><span data-stu-id="faf34-102">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="faf34-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="faf34-103">Permissions</span></span>
<span data-ttu-id="faf34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="faf34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="faf34-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="faf34-106">Permission type</span></span>      | <span data-ttu-id="faf34-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="faf34-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="faf34-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="faf34-108">Delegated (work or school account)</span></span> | <span data-ttu-id="faf34-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf34-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="faf34-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="faf34-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faf34-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faf34-111">Not supported.</span></span>    |
|<span data-ttu-id="faf34-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="faf34-112">Application</span></span> | <span data-ttu-id="faf34-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf34-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="faf34-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="faf34-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="faf34-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="faf34-115">Request headers</span></span>
| <span data-ttu-id="faf34-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="faf34-116">Header</span></span>       | <span data-ttu-id="faf34-117">Valor</span><span class="sxs-lookup"><span data-stu-id="faf34-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="faf34-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="faf34-118">Authorization</span></span>  | <span data-ttu-id="faf34-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="faf34-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="faf34-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="faf34-121">Content-Type</span></span>  | <span data-ttu-id="faf34-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="faf34-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="faf34-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="faf34-124">Request body</span></span>
<span data-ttu-id="faf34-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="faf34-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="faf34-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faf34-128">Property</span></span>     | <span data-ttu-id="faf34-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="faf34-129">Type</span></span>   |<span data-ttu-id="faf34-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="faf34-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faf34-131">isLocked</span><span class="sxs-lookup"><span data-stu-id="faf34-131">isLocked</span></span>|<span data-ttu-id="faf34-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="faf34-132">Boolean</span></span>|<span data-ttu-id="faf34-p105">Indica se o thread está bloqueado. Defina como `true` para proibir a postagem.</span><span class="sxs-lookup"><span data-stu-id="faf34-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="faf34-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="faf34-135">Response</span></span>

<span data-ttu-id="faf34-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faf34-136">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="faf34-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="faf34-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="faf34-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="faf34-138">Request</span></span>
<span data-ttu-id="faf34-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="faf34-139">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="faf34-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="faf34-140">Response</span></span>
<span data-ttu-id="faf34-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="faf34-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
