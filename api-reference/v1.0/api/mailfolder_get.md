# <a name="get-mailfolder"></a><span data-ttu-id="334cb-101">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="334cb-101">Get mailFolder</span></span>

<span data-ttu-id="334cb-102">Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.</span><span class="sxs-lookup"><span data-stu-id="334cb-102">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="334cb-103">Há dois cenários onde um aplicativo pode obter a pasta de correio de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="334cb-103">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="334cb-104">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="334cb-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="334cb-105">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de email com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="334cb-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="334cb-106">Consulte os [detalhes e um exemplo](../../../concepts/outlook-share-messages-folders.md).</span><span class="sxs-lookup"><span data-stu-id="334cb-106">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="334cb-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="334cb-107">Permissions</span></span>
<span data-ttu-id="334cb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="334cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="334cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="334cb-110">Permission type</span></span>      | <span data-ttu-id="334cb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="334cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="334cb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="334cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="334cb-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334cb-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="334cb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="334cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="334cb-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334cb-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="334cb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="334cb-116">Application</span></span> | <span data-ttu-id="334cb-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334cb-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="334cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="334cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="334cb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="334cb-119">Optional query parameters</span></span>
<span data-ttu-id="334cb-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="334cb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="334cb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="334cb-121">Request headers</span></span>
| <span data-ttu-id="334cb-122">Nome</span><span class="sxs-lookup"><span data-stu-id="334cb-122">Name</span></span>       | <span data-ttu-id="334cb-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="334cb-123">Type</span></span> | <span data-ttu-id="334cb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="334cb-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="334cb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="334cb-125">Authorization</span></span>  | <span data-ttu-id="334cb-126">string</span><span class="sxs-lookup"><span data-stu-id="334cb-126">string</span></span>  | <span data-ttu-id="334cb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="334cb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="334cb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="334cb-129">Request body</span></span>
<span data-ttu-id="334cb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="334cb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="334cb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="334cb-131">Response</span></span>

<span data-ttu-id="334cb-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="334cb-132">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="334cb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="334cb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="334cb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="334cb-134">Request</span></span>
<span data-ttu-id="334cb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="334cb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="334cb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="334cb-136">Response</span></span>
<span data-ttu-id="334cb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="334cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
