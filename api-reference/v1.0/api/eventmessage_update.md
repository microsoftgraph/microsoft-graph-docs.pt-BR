# <a name="update-eventmessage"></a><span data-ttu-id="f9625-101">Atualizar eventmessage</span><span class="sxs-lookup"><span data-stu-id="f9625-101">Update eventmessage</span></span>

<span data-ttu-id="f9625-102">Atualiza as propriedades do objeto eventmessage.</span><span class="sxs-lookup"><span data-stu-id="f9625-102">Update the properties of eventmessage object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9625-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9625-103">Prerequisites</span></span>
<span data-ttu-id="f9625-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="f9625-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="f9625-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9625-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f9625-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9625-106">Request headers</span></span>
| <span data-ttu-id="f9625-107">Nome</span><span class="sxs-lookup"><span data-stu-id="f9625-107">Name</span></span>       | <span data-ttu-id="f9625-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9625-108">Type</span></span> | <span data-ttu-id="f9625-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9625-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9625-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9625-110">Authorization</span></span>  | <span data-ttu-id="f9625-111">string</span><span class="sxs-lookup"><span data-stu-id="f9625-111">string</span></span>  | <span data-ttu-id="f9625-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9625-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9625-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9625-114">Content-Type</span></span> | <span data-ttu-id="f9625-115">string</span><span class="sxs-lookup"><span data-stu-id="f9625-115">string</span></span>  | <span data-ttu-id="f9625-p102">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9625-p102">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="f9625-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9625-118">Request body</span></span>
<span data-ttu-id="f9625-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="f9625-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="f9625-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9625-123">Property</span></span>     | <span data-ttu-id="f9625-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9625-124">Type</span></span>   |<span data-ttu-id="f9625-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9625-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9625-126">categories</span><span class="sxs-lookup"><span data-stu-id="f9625-126">categories</span></span>|<span data-ttu-id="f9625-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9625-127">String</span></span>|<span data-ttu-id="f9625-128">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="f9625-128">The categories associated with the message.</span></span>|
|<span data-ttu-id="f9625-129">importance</span><span class="sxs-lookup"><span data-stu-id="f9625-129">importance</span></span>|<span data-ttu-id="f9625-130">String</span><span class="sxs-lookup"><span data-stu-id="f9625-130">String</span></span>|<span data-ttu-id="f9625-p104">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="f9625-p104">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="f9625-133">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f9625-133">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="f9625-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9625-134">Boolean</span></span>|<span data-ttu-id="f9625-135">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="f9625-135">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="f9625-136">isRead</span><span class="sxs-lookup"><span data-stu-id="f9625-136">isRead</span></span>|<span data-ttu-id="f9625-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9625-137">Boolean</span></span>|<span data-ttu-id="f9625-138">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="f9625-138">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="f9625-139">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f9625-139">isReadReceiptRequested</span></span>|<span data-ttu-id="f9625-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9625-140">Boolean</span></span>|<span data-ttu-id="f9625-141">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="f9625-141">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="f9625-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9625-142">Response</span></span>

<span data-ttu-id="f9625-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9625-143">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9625-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9625-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9625-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9625-145">Request</span></span>
<span data-ttu-id="f9625-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9625-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="f9625-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9625-147">Response</span></span>
<span data-ttu-id="f9625-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9625-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
