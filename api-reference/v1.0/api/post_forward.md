# <a name="post-forward"></a><span data-ttu-id="997b7-101">post: forward</span><span class="sxs-lookup"><span data-stu-id="997b7-101">post: forward</span></span>

<span data-ttu-id="997b7-p101">Encaminhe uma postagem para um destinatário. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="997b7-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="997b7-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="997b7-104">Permissions</span></span>
<span data-ttu-id="997b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="997b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="997b7-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="997b7-107">Permission type</span></span>      | <span data-ttu-id="997b7-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="997b7-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="997b7-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="997b7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="997b7-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="997b7-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="997b7-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="997b7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="997b7-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="997b7-112">Not supported.</span></span>    | 
|<span data-ttu-id="997b7-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="997b7-113">Application</span></span> | <span data-ttu-id="997b7-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="997b7-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="997b7-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="997b7-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="997b7-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="997b7-116">Request headers</span></span>
| <span data-ttu-id="997b7-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="997b7-117">Header</span></span>       | <span data-ttu-id="997b7-118">Valor</span><span class="sxs-lookup"><span data-stu-id="997b7-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="997b7-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="997b7-119">Authorization</span></span>  | <span data-ttu-id="997b7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="997b7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="997b7-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="997b7-122">Request body</span></span>
<span data-ttu-id="997b7-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="997b7-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="997b7-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="997b7-124">Parameter</span></span>    | <span data-ttu-id="997b7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="997b7-125">Type</span></span>   |<span data-ttu-id="997b7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="997b7-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="997b7-127">comment</span><span class="sxs-lookup"><span data-stu-id="997b7-127">comment</span></span>|<span data-ttu-id="997b7-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="997b7-128">String</span></span>|<span data-ttu-id="997b7-129">Comentário opcional que é encaminhado com a postagem.</span><span class="sxs-lookup"><span data-stu-id="997b7-129">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="997b7-130">toRecipients</span><span class="sxs-lookup"><span data-stu-id="997b7-130">toRecipients</span></span>|<span data-ttu-id="997b7-131">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="997b7-131">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="997b7-132">Os destinatários aos quais os threads são encaminhados.</span><span class="sxs-lookup"><span data-stu-id="997b7-132">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="997b7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="997b7-133">Response</span></span>

<span data-ttu-id="997b7-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="997b7-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="997b7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="997b7-136">Example</span></span>
<span data-ttu-id="997b7-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="997b7-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="997b7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="997b7-138">Request</span></span>
<span data-ttu-id="997b7-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="997b7-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="997b7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="997b7-140">Response</span></span>
<span data-ttu-id="997b7-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="997b7-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
