# <a name="message-reply"></a><span data-ttu-id="7452c-101">message: reply</span><span class="sxs-lookup"><span data-stu-id="7452c-101">message: reply</span></span>

<span data-ttu-id="7452c-p101">Responda ao remetente de uma mensagem A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="7452c-p101">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7452c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7452c-104">Prerequisites</span></span>
<span data-ttu-id="7452c-105">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="7452c-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="7452c-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7452c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="7452c-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7452c-107">Request headers</span></span>
| <span data-ttu-id="7452c-108">Nome</span><span class="sxs-lookup"><span data-stu-id="7452c-108">Name</span></span>       | <span data-ttu-id="7452c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7452c-109">Type</span></span> | <span data-ttu-id="7452c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7452c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7452c-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="7452c-111">Authorization</span></span>  | <span data-ttu-id="7452c-112">string</span><span class="sxs-lookup"><span data-stu-id="7452c-112">string</span></span>  | <span data-ttu-id="7452c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7452c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7452c-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7452c-115">Content-Type</span></span> | <span data-ttu-id="7452c-116">string</span><span class="sxs-lookup"><span data-stu-id="7452c-116">string</span></span>  | <span data-ttu-id="7452c-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7452c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7452c-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7452c-119">Request body</span></span>
<span data-ttu-id="7452c-120">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7452c-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7452c-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7452c-121">Parameter</span></span>    | <span data-ttu-id="7452c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7452c-122">Type</span></span>   |<span data-ttu-id="7452c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7452c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7452c-124">comment</span><span class="sxs-lookup"><span data-stu-id="7452c-124">comment</span></span>|<span data-ttu-id="7452c-125">String</span><span class="sxs-lookup"><span data-stu-id="7452c-125">String</span></span>|<span data-ttu-id="7452c-p104">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="7452c-p104">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="7452c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7452c-128">Response</span></span>

<span data-ttu-id="7452c-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7452c-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7452c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7452c-131">Example</span></span>
<span data-ttu-id="7452c-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7452c-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7452c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7452c-133">Request</span></span>
<span data-ttu-id="7452c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7452c-134">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7452c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7452c-135">Response</span></span>
##### <a name="response"></a><span data-ttu-id="7452c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7452c-136">Response</span></span>
<span data-ttu-id="7452c-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7452c-137">Here is an example of the response.</span></span>
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
