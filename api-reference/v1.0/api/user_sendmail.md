# <a name="send-mail"></a><span data-ttu-id="5e094-101">Enviar email</span><span class="sxs-lookup"><span data-stu-id="5e094-101">Send mail</span></span>

<span data-ttu-id="5e094-p101">Enviar a mensagem especificada no corpo da solicitação. A mensagem é salva na pasta Itens Enviados por padrão.</span><span class="sxs-lookup"><span data-stu-id="5e094-p101">Send the message specified in the request body. The message is saved in the Sent Items folder by default.</span></span>

<span data-ttu-id="5e094-104">Você pode incluir um [anexo de arquivo](../resources/fileattachment.md) na mesma chamada de ação de **sendMail**.</span><span class="sxs-lookup"><span data-stu-id="5e094-104">You can include a [file attachment](../resources/fileattachment.md) in the same **sendMail** action call.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e094-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e094-105">Prerequisites</span></span>
<span data-ttu-id="5e094-106">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="5e094-106">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>

## <a name="http-request"></a><span data-ttu-id="5e094-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e094-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/sendMail
```
## <a name="request-headers"></a><span data-ttu-id="5e094-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e094-108">Request headers</span></span>
| <span data-ttu-id="5e094-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e094-109">Header</span></span>       | <span data-ttu-id="5e094-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5e094-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e094-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e094-111">Authorization</span></span>  | <span data-ttu-id="5e094-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e094-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e094-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e094-114">Content-Type</span></span>  | <span data-ttu-id="5e094-115">application/json</span><span class="sxs-lookup"><span data-stu-id="5e094-115">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e094-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e094-116">Request body</span></span>
<span data-ttu-id="5e094-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e094-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e094-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5e094-118">Parameter</span></span>    | <span data-ttu-id="5e094-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e094-119">Type</span></span>   |<span data-ttu-id="5e094-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e094-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e094-121">Message</span><span class="sxs-lookup"><span data-stu-id="5e094-121">Message</span></span>|[<span data-ttu-id="5e094-122">Message</span><span class="sxs-lookup"><span data-stu-id="5e094-122">Message</span></span>](../resources/message.md)|<span data-ttu-id="5e094-p103">A mensagem a enviar. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e094-p103">The message to send. Required.</span></span>|
|<span data-ttu-id="5e094-125">SaveToSentItems</span><span class="sxs-lookup"><span data-stu-id="5e094-125">SaveToSentItems</span></span>|<span data-ttu-id="5e094-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e094-126">Boolean</span></span>|<span data-ttu-id="5e094-p104">Indica se é necessário salvar a mensagem nos Itens Enviados. Especifique-a somente se o parâmetro for false; o padrão é true.  Opcional.</span><span class="sxs-lookup"><span data-stu-id="5e094-p104">Indicates whether to save the message in Sent Items. Specify it only if the parameter is false; default is true.  Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5e094-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e094-130">Response</span></span>

<span data-ttu-id="5e094-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e094-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e094-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e094-133">Example</span></span>
<span data-ttu-id="5e094-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5e094-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5e094-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e094-135">Request</span></span>
<span data-ttu-id="5e094-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e094-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5e094-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e094-137">Response</span></span>
<span data-ttu-id="5e094-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e094-138">Here is an example of the response.</span></span>
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
