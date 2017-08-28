# <a name="update-eventmessage"></a><span data-ttu-id="5f86a-101">Atualizar eventmessage</span><span class="sxs-lookup"><span data-stu-id="5f86a-101">Update eventmessage</span></span>

<span data-ttu-id="5f86a-102">Atualizar as propriedades do objeto eventmessage.</span><span class="sxs-lookup"><span data-stu-id="5f86a-102">Update the properties of eventmessage object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f86a-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f86a-103">Permissions</span></span>
<span data-ttu-id="5f86a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f86a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5f86a-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f86a-106">Permission type</span></span>      | <span data-ttu-id="5f86a-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f86a-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="5f86a-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f86a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5f86a-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f86a-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="5f86a-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f86a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f86a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f86a-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="5f86a-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f86a-112">Application</span></span> | <span data-ttu-id="5f86a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f86a-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5f86a-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f86a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5f86a-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f86a-115">Request headers</span></span>
| <span data-ttu-id="5f86a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="5f86a-116">Name</span></span>       | <span data-ttu-id="5f86a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f86a-117">Type</span></span> | <span data-ttu-id="5f86a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f86a-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5f86a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f86a-119">Authorization</span></span>  | <span data-ttu-id="5f86a-120">string</span><span class="sxs-lookup"><span data-stu-id="5f86a-120">string</span></span>  | <span data-ttu-id="5f86a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f86a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f86a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f86a-123">Content-Type</span></span> | <span data-ttu-id="5f86a-124">string</span><span class="sxs-lookup"><span data-stu-id="5f86a-124">string</span></span>  | <span data-ttu-id="5f86a-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f86a-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="5f86a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f86a-127">Request body</span></span>
<span data-ttu-id="5f86a-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são</span><span class="sxs-lookup"><span data-stu-id="5f86a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="5f86a-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f86a-132">Property</span></span>     | <span data-ttu-id="5f86a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f86a-133">Type</span></span>   |<span data-ttu-id="5f86a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f86a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f86a-135">categories</span><span class="sxs-lookup"><span data-stu-id="5f86a-135">categories</span></span>|<span data-ttu-id="5f86a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f86a-136">String</span></span>|<span data-ttu-id="5f86a-137">As categorias associadas à mensagem.</span><span class="sxs-lookup"><span data-stu-id="5f86a-137">The categories associated with the message.</span></span>|
|<span data-ttu-id="5f86a-138">importance</span><span class="sxs-lookup"><span data-stu-id="5f86a-138">importance</span></span>|<span data-ttu-id="5f86a-139">String</span><span class="sxs-lookup"><span data-stu-id="5f86a-139">String</span></span>|<span data-ttu-id="5f86a-p105">A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.</span><span class="sxs-lookup"><span data-stu-id="5f86a-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="5f86a-142">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="5f86a-142">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="5f86a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f86a-143">Boolean</span></span>|<span data-ttu-id="5f86a-144">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="5f86a-144">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="5f86a-145">isRead</span><span class="sxs-lookup"><span data-stu-id="5f86a-145">isRead</span></span>|<span data-ttu-id="5f86a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f86a-146">Boolean</span></span>|<span data-ttu-id="5f86a-147">Indica se a mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="5f86a-147">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="5f86a-148">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="5f86a-148">isReadReceiptRequested</span></span>|<span data-ttu-id="5f86a-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f86a-149">Boolean</span></span>|<span data-ttu-id="5f86a-150">Indica se uma confirmação de leitura foi solicitada para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="5f86a-150">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="5f86a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f86a-151">Response</span></span>

<span data-ttu-id="5f86a-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f86a-152">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f86a-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f86a-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f86a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f86a-154">Request</span></span>
<span data-ttu-id="5f86a-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f86a-155">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5f86a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f86a-156">Response</span></span>
<span data-ttu-id="5f86a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f86a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
