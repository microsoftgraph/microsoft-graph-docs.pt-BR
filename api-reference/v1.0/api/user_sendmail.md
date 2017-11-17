# <a name="send-mail"></a><span data-ttu-id="9627e-101">Enviar email</span><span class="sxs-lookup"><span data-stu-id="9627e-101">Send mail</span></span>

<span data-ttu-id="9627e-p101">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="9627e-p101">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="9627e-104">Você pode incluir um [anexo de arquivo](../resources/fileattachment.md) na mesma chamada de ação de **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="9627e-104">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="permissions"></a><span data-ttu-id="9627e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9627e-105">Permissions</span></span>
<span data-ttu-id="9627e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9627e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9627e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9627e-108">Permission type</span></span>      | <span data-ttu-id="9627e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9627e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9627e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9627e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9627e-111">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9627e-111">Mail.Send</span></span>    |
|<span data-ttu-id="9627e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9627e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9627e-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9627e-113">Mail.Send</span></span>    |
|<span data-ttu-id="9627e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9627e-114">Application</span></span> | <span data-ttu-id="9627e-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9627e-115">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9627e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9627e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="9627e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9627e-117">Request headers</span></span>
| <span data-ttu-id="9627e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9627e-118">Header</span></span>       | <span data-ttu-id="9627e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="9627e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9627e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9627e-120">Authorization</span></span>  | <span data-ttu-id="9627e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9627e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9627e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9627e-123">Content-Type</span></span>  | <span data-ttu-id="9627e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9627e-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9627e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9627e-125">Request body</span></span>
<span data-ttu-id="9627e-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9627e-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9627e-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9627e-127">Parameter</span></span>    | <span data-ttu-id="9627e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="9627e-128">Type</span></span>   |<span data-ttu-id="9627e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="9627e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9627e-130">Message</span><span class="sxs-lookup"><span data-stu-id="9627e-130">Message</span></span>|[<span data-ttu-id="9627e-131">Message</span><span class="sxs-lookup"><span data-stu-id="9627e-131">Message</span></span>](../resources/message.md)|<span data-ttu-id="9627e-p104">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9627e-p104">The message to send. Required.</span></span>|
|<span data-ttu-id="9627e-134">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="9627e-134">SaveToSentItems</span></span>|<span data-ttu-id="9627e-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="9627e-135">Boolean</span></span>|<span data-ttu-id="9627e-p105">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="9627e-p105">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9627e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9627e-139">Response</span></span>

<span data-ttu-id="9627e-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9627e-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9627e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9627e-142">Example</span></span>
<span data-ttu-id="9627e-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9627e-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9627e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9627e-144">Request</span></span>
<span data-ttu-id="9627e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9627e-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <a name="response"></a><span data-ttu-id="9627e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9627e-146">Response</span></span>
<span data-ttu-id="9627e-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9627e-147">Here is an example of the response.</span></span>
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
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
