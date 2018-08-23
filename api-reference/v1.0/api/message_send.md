# <a name="message-send"></a><span data-ttu-id="1ad61-101">message: send</span><span class="sxs-lookup"><span data-stu-id="1ad61-101">message: send</span></span>

<span data-ttu-id="1ad61-p101">Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="1ad61-p101">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ad61-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ad61-105">Permissions</span></span>

<span data-ttu-id="1ad61-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ad61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1ad61-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ad61-108">Permission type</span></span>      | <span data-ttu-id="1ad61-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ad61-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ad61-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ad61-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ad61-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1ad61-111">Mail.Send</span></span>    |
|<span data-ttu-id="1ad61-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ad61-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ad61-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1ad61-113">Mail.Send</span></span>    |
|<span data-ttu-id="1ad61-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ad61-114">Application</span></span> | <span data-ttu-id="1ad61-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1ad61-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ad61-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ad61-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="1ad61-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ad61-117">Request headers</span></span>

| <span data-ttu-id="1ad61-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1ad61-118">Name</span></span>       | <span data-ttu-id="1ad61-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ad61-119">Type</span></span> | <span data-ttu-id="1ad61-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ad61-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1ad61-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ad61-121">Authorization</span></span>  | <span data-ttu-id="1ad61-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ad61-122">string</span></span>  | <span data-ttu-id="1ad61-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ad61-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ad61-125">Tamanho do conteúdo</span><span class="sxs-lookup"><span data-stu-id="1ad61-125">Content-Length</span></span> | <span data-ttu-id="1ad61-126">número</span><span class="sxs-lookup"><span data-stu-id="1ad61-126">number</span></span> | <span data-ttu-id="1ad61-127">0. Necessário.</span><span class="sxs-lookup"><span data-stu-id="1ad61-127">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ad61-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ad61-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1ad61-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ad61-129">Response</span></span>

<span data-ttu-id="1ad61-p104">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ad61-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ad61-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ad61-132">Example</span></span>

<span data-ttu-id="1ad61-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1ad61-133">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1ad61-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ad61-134">Request</span></span>

<span data-ttu-id="1ad61-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ad61-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="1ad61-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ad61-136">Response</span></span>

<span data-ttu-id="1ad61-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ad61-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
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
