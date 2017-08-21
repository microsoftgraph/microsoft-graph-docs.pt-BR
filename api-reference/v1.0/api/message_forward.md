# <a name="message-forward"></a><span data-ttu-id="8cb5a-101">message: forward</span><span class="sxs-lookup"><span data-stu-id="8cb5a-101">message: forward</span></span>

<span data-ttu-id="8cb5a-p101">Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cb5a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cb5a-104">Prerequisites</span></span>
<span data-ttu-id="8cb5a-105">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="8cb5a-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="8cb5a-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cb5a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="8cb5a-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb5a-107">Request headers</span></span>
| <span data-ttu-id="8cb5a-108">Nome</span><span class="sxs-lookup"><span data-stu-id="8cb5a-108">Name</span></span>       | <span data-ttu-id="8cb5a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cb5a-109">Type</span></span> | <span data-ttu-id="8cb5a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cb5a-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8cb5a-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cb5a-111">Authorization</span></span>  | <span data-ttu-id="8cb5a-112">string</span><span class="sxs-lookup"><span data-stu-id="8cb5a-112">string</span></span>  | <span data-ttu-id="8cb5a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8cb5a-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cb5a-115">Content-Type</span></span> | <span data-ttu-id="8cb5a-116">string</span><span class="sxs-lookup"><span data-stu-id="8cb5a-116">string</span></span>  | <span data-ttu-id="8cb5a-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cb5a-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb5a-119">Request body</span></span>
<span data-ttu-id="8cb5a-120">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8cb5a-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8cb5a-121">Parameter</span></span>    | <span data-ttu-id="8cb5a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cb5a-122">Type</span></span>   |<span data-ttu-id="8cb5a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cb5a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cb5a-124">comment</span><span class="sxs-lookup"><span data-stu-id="8cb5a-124">comment</span></span>|<span data-ttu-id="8cb5a-125">String</span><span class="sxs-lookup"><span data-stu-id="8cb5a-125">String</span></span>|<span data-ttu-id="8cb5a-p104">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-p104">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="8cb5a-128">toRecipients</span><span class="sxs-lookup"><span data-stu-id="8cb5a-128">toRecipients</span></span>|<span data-ttu-id="8cb5a-129">Coleção [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="8cb5a-129">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="8cb5a-130">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-130">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="8cb5a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb5a-131">Response</span></span>

<span data-ttu-id="8cb5a-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb5a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cb5a-134">Example</span></span>
<span data-ttu-id="8cb5a-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8cb5a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb5a-136">Request</span></span>
<span data-ttu-id="8cb5a-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="8cb5a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb5a-138">Response</span></span>
##### <a name="response"></a><span data-ttu-id="8cb5a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb5a-139">Response</span></span>
<span data-ttu-id="8cb5a-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cb5a-140">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
