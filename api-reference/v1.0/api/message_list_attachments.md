# <a name="list-attachments"></a><span data-ttu-id="b05ce-101">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="b05ce-101">List attachments</span></span>

<span data-ttu-id="b05ce-102">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b05ce-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="b05ce-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b05ce-103">Permissions</span></span>
<span data-ttu-id="b05ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b05ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b05ce-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b05ce-106">Permission type</span></span>      | <span data-ttu-id="b05ce-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b05ce-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b05ce-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b05ce-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b05ce-109">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b05ce-109">Mail.Read</span></span>    |
|<span data-ttu-id="b05ce-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b05ce-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b05ce-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b05ce-111">Mail.Read</span></span>    |
|<span data-ttu-id="b05ce-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b05ce-112">Application</span></span> | <span data-ttu-id="b05ce-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b05ce-113">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b05ce-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b05ce-114">HTTP request</span></span>
<span data-ttu-id="b05ce-115"><!-- { "blockType": "ignored" } -->Anexos de uma [mensagem](../resources/message.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="b05ce-115"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="b05ce-116">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b05ce-116">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="b05ce-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="b05ce-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b05ce-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b05ce-119">Optional query parameters</span></span>
<span data-ttu-id="b05ce-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b05ce-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b05ce-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b05ce-121">Request headers</span></span>
| <span data-ttu-id="b05ce-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b05ce-122">Name</span></span>       | <span data-ttu-id="b05ce-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b05ce-123">Type</span></span> | <span data-ttu-id="b05ce-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b05ce-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b05ce-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b05ce-125">Authorization</span></span>  | <span data-ttu-id="b05ce-126">string</span><span class="sxs-lookup"><span data-stu-id="b05ce-126">string</span></span>  | <span data-ttu-id="b05ce-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b05ce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b05ce-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b05ce-129">Request body</span></span>
<span data-ttu-id="b05ce-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b05ce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b05ce-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b05ce-131">Response</span></span>

<span data-ttu-id="b05ce-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b05ce-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b05ce-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b05ce-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b05ce-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b05ce-134">Request</span></span>
<span data-ttu-id="b05ce-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b05ce-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="b05ce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b05ce-136">Response</span></span>
<span data-ttu-id="b05ce-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b05ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->