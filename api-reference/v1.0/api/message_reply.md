# <a name="message-reply"></a><span data-ttu-id="564e1-101">message: reply</span><span class="sxs-lookup"><span data-stu-id="564e1-101">message: reply</span></span>

<span data-ttu-id="564e1-p101">Responda ao remetente de uma mensagem A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="564e1-p101">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="564e1-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="564e1-104">Permissions</span></span>
<span data-ttu-id="564e1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="564e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="564e1-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="564e1-107">Permission type</span></span>      | <span data-ttu-id="564e1-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="564e1-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="564e1-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="564e1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="564e1-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="564e1-110">Mail.Send</span></span>    |
|<span data-ttu-id="564e1-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="564e1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="564e1-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="564e1-112">Mail.Send</span></span>    |
|<span data-ttu-id="564e1-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="564e1-113">Application</span></span> | <span data-ttu-id="564e1-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="564e1-114">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="564e1-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="564e1-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="564e1-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="564e1-116">Request headers</span></span>
| <span data-ttu-id="564e1-117">Nome</span><span class="sxs-lookup"><span data-stu-id="564e1-117">Name</span></span>       | <span data-ttu-id="564e1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="564e1-118">Type</span></span> | <span data-ttu-id="564e1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="564e1-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="564e1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="564e1-120">Authorization</span></span>  | <span data-ttu-id="564e1-121">string</span><span class="sxs-lookup"><span data-stu-id="564e1-121">string</span></span>  | <span data-ttu-id="564e1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="564e1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="564e1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="564e1-124">Content-Type</span></span> | <span data-ttu-id="564e1-125">string</span><span class="sxs-lookup"><span data-stu-id="564e1-125">string</span></span>  | <span data-ttu-id="564e1-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="564e1-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="564e1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="564e1-128">Request body</span></span>
<span data-ttu-id="564e1-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="564e1-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="564e1-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="564e1-130">Parameter</span></span>    | <span data-ttu-id="564e1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="564e1-131">Type</span></span>   |<span data-ttu-id="564e1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="564e1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="564e1-133">comment</span><span class="sxs-lookup"><span data-stu-id="564e1-133">comment</span></span>|<span data-ttu-id="564e1-134">String</span><span class="sxs-lookup"><span data-stu-id="564e1-134">String</span></span>|<span data-ttu-id="564e1-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="564e1-p105">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="564e1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="564e1-137">Response</span></span>

<span data-ttu-id="564e1-p106">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="564e1-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="564e1-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="564e1-140">Example</span></span>
<span data-ttu-id="564e1-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="564e1-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="564e1-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="564e1-142">Request</span></span>
<span data-ttu-id="564e1-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="564e1-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="564e1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="564e1-144">Response</span></span>
##### <a name="response"></a><span data-ttu-id="564e1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="564e1-145">Response</span></span>
<span data-ttu-id="564e1-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="564e1-146">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
