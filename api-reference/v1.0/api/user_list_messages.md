# <a name="list-messages"></a><span data-ttu-id="e4d13-101">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="e4d13-101">List messages</span></span>

<span data-ttu-id="e4d13-102">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="e4d13-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="e4d13-103">No momento, essa operação retorna corpos de mensagens somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="e4d13-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="e4d13-104">Há dois cenários onde um aplicativo pode obter mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="e4d13-104">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="e4d13-105">Se o aplicativo tiver permissões de aplicativo ou,</span><span class="sxs-lookup"><span data-stu-id="e4d13-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="e4d13-106">Se o aplicativo tiver as [permissões](#permissions) apropriadas delegadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com o primeiro usuário ou, tiver dado acesso delegado a ele.</span><span class="sxs-lookup"><span data-stu-id="e4d13-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="e4d13-107">Confira os [detalhes e um exemplo](../../../concepts/outlook-share-messages-folders.md).</span><span class="sxs-lookup"><span data-stu-id="e4d13-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4d13-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4d13-108">Permissions</span></span>
<span data-ttu-id="e4d13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4d13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4d13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4d13-111">Permission type</span></span>      | <span data-ttu-id="e4d13-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4d13-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4d13-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4d13-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e4d13-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d13-114">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e4d13-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4d13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4d13-116">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d13-116">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e4d13-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4d13-117">Application</span></span> | <span data-ttu-id="e4d13-118">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d13-118">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4d13-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4d13-119">HTTP request</span></span>

<span data-ttu-id="e4d13-120">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="e4d13-120">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="e4d13-121">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="e4d13-121">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4d13-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e4d13-122">Optional query parameters</span></span>
<span data-ttu-id="e4d13-123">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e4d13-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e4d13-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4d13-124">Request headers</span></span>
| <span data-ttu-id="e4d13-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e4d13-125">Name</span></span>       | <span data-ttu-id="e4d13-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4d13-126">Type</span></span> | <span data-ttu-id="e4d13-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4d13-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e4d13-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4d13-128">Authorization</span></span>  | <span data-ttu-id="e4d13-129">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4d13-129">string</span></span>  | <span data-ttu-id="e4d13-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4d13-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4d13-132">Preferir: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="e4d13-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="e4d13-133">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4d13-133">string</span></span> | <span data-ttu-id="e4d13-134">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="e4d13-134">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="e4d13-135">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="e4d13-135">Values can be "text" or "html".</span></span> <span data-ttu-id="e4d13-136">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="e4d13-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="e4d13-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e4d13-137">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e4d13-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4d13-138">Request body</span></span>
<span data-ttu-id="e4d13-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4d13-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4d13-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4d13-140">Response</span></span>

<span data-ttu-id="e4d13-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4d13-141">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="e4d13-142">O tamanho de página padrão para essa solicitação é dez mensagens.</span><span class="sxs-lookup"><span data-stu-id="e4d13-142">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="e4d13-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4d13-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4d13-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4d13-144">Request</span></span>
<span data-ttu-id="e4d13-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4d13-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="e4d13-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4d13-146">Response</span></span>
<span data-ttu-id="e4d13-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4d13-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
