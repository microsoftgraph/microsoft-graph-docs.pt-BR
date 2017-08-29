# <a name="message-forward"></a><span data-ttu-id="38646-101">message: forward</span><span class="sxs-lookup"><span data-stu-id="38646-101">message: forward</span></span>

<span data-ttu-id="38646-p101">Encaminhe uma mensagem. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="38646-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="38646-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="38646-104">Permissions</span></span>
<span data-ttu-id="38646-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38646-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="38646-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38646-107">Permission type</span></span>      | <span data-ttu-id="38646-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38646-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38646-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38646-109">Delegated (work or school account)</span></span> | <span data-ttu-id="38646-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="38646-110">Mail.Send</span></span>    |
|<span data-ttu-id="38646-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38646-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38646-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="38646-112">Mail.Send</span></span>    |
|<span data-ttu-id="38646-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38646-113">Application</span></span> | <span data-ttu-id="38646-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="38646-114">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="38646-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38646-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="38646-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38646-116">Request headers</span></span>
| <span data-ttu-id="38646-117">Nome</span><span class="sxs-lookup"><span data-stu-id="38646-117">Name</span></span>       | <span data-ttu-id="38646-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="38646-118">Type</span></span> | <span data-ttu-id="38646-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="38646-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38646-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="38646-120">Authorization</span></span>  | <span data-ttu-id="38646-121">string</span><span class="sxs-lookup"><span data-stu-id="38646-121">string</span></span>  | <span data-ttu-id="38646-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38646-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38646-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38646-124">Content-Type</span></span> | <span data-ttu-id="38646-125">string</span><span class="sxs-lookup"><span data-stu-id="38646-125">string</span></span>  | <span data-ttu-id="38646-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38646-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38646-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38646-128">Request body</span></span>
<span data-ttu-id="38646-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38646-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="38646-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="38646-130">Parameter</span></span>    | <span data-ttu-id="38646-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="38646-131">Type</span></span>   |<span data-ttu-id="38646-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="38646-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38646-133">comment</span><span class="sxs-lookup"><span data-stu-id="38646-133">comment</span></span>|<span data-ttu-id="38646-134">String</span><span class="sxs-lookup"><span data-stu-id="38646-134">String</span></span>|<span data-ttu-id="38646-p105">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="38646-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="38646-137">toRecipients</span><span class="sxs-lookup"><span data-stu-id="38646-137">toRecipients</span></span>|<span data-ttu-id="38646-138">Coleção [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="38646-138">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="38646-139">A lista de destinatários.</span><span class="sxs-lookup"><span data-stu-id="38646-139">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="38646-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="38646-140">Response</span></span>

<span data-ttu-id="38646-p106">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38646-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38646-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38646-143">Example</span></span>
<span data-ttu-id="38646-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="38646-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38646-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38646-145">Request</span></span>
<span data-ttu-id="38646-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38646-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="38646-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="38646-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="38646-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="38646-148">Response</span></span>
<span data-ttu-id="38646-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38646-149">Here is an example of the response.</span></span>
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
