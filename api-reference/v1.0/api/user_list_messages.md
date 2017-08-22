# <a name="list-messages"></a><span data-ttu-id="23745-101">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="23745-101">List messages</span></span>

<span data-ttu-id="23745-102">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="23745-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="23745-103">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="23745-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23745-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23745-104">Prerequisites</span></span>
<span data-ttu-id="23745-105">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Read; Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="23745-105">One of the following scopes is required to execute this API: Mail.Read; Mail.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="23745-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23745-106">HTTP request</span></span>

<span data-ttu-id="23745-107">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="23745-107">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="23745-108">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="23745-108">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23745-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23745-109">Optional query parameters</span></span>
<span data-ttu-id="23745-110">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23745-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23745-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23745-111">Request headers</span></span>
| <span data-ttu-id="23745-112">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23745-112">Header</span></span>       | <span data-ttu-id="23745-113">Valor</span><span class="sxs-lookup"><span data-stu-id="23745-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="23745-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="23745-114">Authorization</span></span>  | <span data-ttu-id="23745-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23745-p101">Bearer {token}. Required.</span></span>  |
 

## <a name="request-body"></a><span data-ttu-id="23745-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23745-117">Request body</span></span>
<span data-ttu-id="23745-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23745-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23745-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="23745-119">Response</span></span>

<span data-ttu-id="23745-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23745-120">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="23745-121">O tamanho de página padrão para essa solicitação é dez mensagens.</span><span class="sxs-lookup"><span data-stu-id="23745-121">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="23745-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23745-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23745-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23745-123">Request</span></span>
<span data-ttu-id="23745-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23745-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="23745-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="23745-125">Response</span></span>
<span data-ttu-id="23745-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23745-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
