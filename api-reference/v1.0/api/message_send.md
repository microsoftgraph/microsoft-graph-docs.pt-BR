# <a name="message-send"></a><span data-ttu-id="67d59-101">message: send</span><span class="sxs-lookup"><span data-stu-id="67d59-101">message: send</span></span>

<span data-ttu-id="67d59-p101">Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="67d59-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67d59-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67d59-105">Prerequisites</span></span>
<span data-ttu-id="67d59-106">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="67d59-106">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="67d59-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67d59-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```
## <a name="request-headers"></a><span data-ttu-id="67d59-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67d59-108">Request headers</span></span>
| <span data-ttu-id="67d59-109">Nome</span><span class="sxs-lookup"><span data-stu-id="67d59-109">Name</span></span>       | <span data-ttu-id="67d59-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="67d59-110">Type</span></span> | <span data-ttu-id="67d59-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67d59-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67d59-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="67d59-112">Authorization</span></span>  | <span data-ttu-id="67d59-113">string</span><span class="sxs-lookup"><span data-stu-id="67d59-113">string</span></span>  | <span data-ttu-id="67d59-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67d59-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67d59-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67d59-116">Request body</span></span>

## <a name="response"></a><span data-ttu-id="67d59-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="67d59-117">Response</span></span>

<span data-ttu-id="67d59-p103">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67d59-p103">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67d59-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67d59-120">Example</span></span>
<span data-ttu-id="67d59-121">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="67d59-121">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="67d59-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67d59-122">Request</span></span>
<span data-ttu-id="67d59-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67d59-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="67d59-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="67d59-124">Response</span></span>
##### <a name="response"></a><span data-ttu-id="67d59-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="67d59-125">Response</span></span>
<span data-ttu-id="67d59-126">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67d59-126">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
