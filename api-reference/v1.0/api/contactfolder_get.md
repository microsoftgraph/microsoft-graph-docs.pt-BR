# <a name="get-contactfolder"></a><span data-ttu-id="8c325-101">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="8c325-101">Get contactFolder</span></span>

<span data-ttu-id="8c325-102">Obter uma pasta de contatos usando o seu ID.</span><span class="sxs-lookup"><span data-stu-id="8c325-102">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="8c325-103">Há dois cenários em que um aplicativo pode obter um contato da pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="8c325-103">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="8c325-104">Se o aplicativo tiver permissões de aplicativo ou,</span><span class="sxs-lookup"><span data-stu-id="8c325-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="8c325-105">Se o aplicativo tiver as [permissões](#permissions) apropriadas delegadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com o primeiro usuário ou, tiver dado acesso delegado a ele.</span><span class="sxs-lookup"><span data-stu-id="8c325-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="8c325-106">Confira os [detalhes e um exemplo](../../../concepts/outlook-get-shared-contacts-folders.md).</span><span class="sxs-lookup"><span data-stu-id="8c325-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="8c325-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c325-107">Permissions</span></span>
<span data-ttu-id="8c325-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c325-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c325-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c325-110">Permission type</span></span>      | <span data-ttu-id="8c325-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c325-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c325-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c325-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c325-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c325-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8c325-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c325-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c325-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c325-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8c325-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c325-116">Application</span></span> | <span data-ttu-id="8c325-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c325-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c325-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c325-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c325-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8c325-119">Optional query parameters</span></span>
<span data-ttu-id="8c325-120">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8c325-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c325-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c325-121">Request headers</span></span>
| <span data-ttu-id="8c325-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8c325-122">Name</span></span>       | <span data-ttu-id="8c325-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c325-123">Type</span></span> | <span data-ttu-id="8c325-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c325-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8c325-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c325-125">Authorization</span></span>  | <span data-ttu-id="8c325-126">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c325-126">string</span></span>  | <span data-ttu-id="8c325-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c325-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c325-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c325-129">Request body</span></span>
<span data-ttu-id="8c325-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c325-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c325-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c325-131">Response</span></span>

<span data-ttu-id="8c325-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c325-132">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c325-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c325-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c325-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c325-134">Request</span></span>
<span data-ttu-id="8c325-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c325-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="8c325-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c325-136">Response</span></span>
<span data-ttu-id="8c325-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c325-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
