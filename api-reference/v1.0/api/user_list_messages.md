# <a name="list-messages"></a><span data-ttu-id="14ad8-101">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="14ad8-101">List messages</span></span>

<span data-ttu-id="14ad8-102">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="14ad8-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="14ad8-103">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="14ad8-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="14ad8-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="14ad8-104">Permissions</span></span>
<span data-ttu-id="14ad8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="14ad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="14ad8-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14ad8-107">Permission type</span></span>      | <span data-ttu-id="14ad8-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14ad8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14ad8-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14ad8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="14ad8-110">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14ad8-110">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="14ad8-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14ad8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14ad8-112">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14ad8-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="14ad8-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14ad8-113">Application</span></span> | <span data-ttu-id="14ad8-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14ad8-114">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="14ad8-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14ad8-115">HTTP request</span></span>

<span data-ttu-id="14ad8-116">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="14ad8-116">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="14ad8-117">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="14ad8-117">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14ad8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="14ad8-118">Optional query parameters</span></span>
<span data-ttu-id="14ad8-119">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="14ad8-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="14ad8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14ad8-120">Request headers</span></span>
| <span data-ttu-id="14ad8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14ad8-121">Header</span></span>       | <span data-ttu-id="14ad8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="14ad8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14ad8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="14ad8-123">Authorization</span></span>  | <span data-ttu-id="14ad8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14ad8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14ad8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14ad8-126">Request body</span></span>
<span data-ttu-id="14ad8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14ad8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14ad8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ad8-128">Response</span></span>

<span data-ttu-id="14ad8-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14ad8-129">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="14ad8-130">O tamanho de página padrão para essa solicitação é dez mensagens.</span><span class="sxs-lookup"><span data-stu-id="14ad8-130">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="14ad8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14ad8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14ad8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14ad8-132">Request</span></span>
<span data-ttu-id="14ad8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14ad8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="14ad8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ad8-134">Response</span></span>
<span data-ttu-id="14ad8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14ad8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
