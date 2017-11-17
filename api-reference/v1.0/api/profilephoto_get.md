# <a name="get-photo"></a><span data-ttu-id="aa7d4-101">Obter foto</span><span class="sxs-lookup"><span data-stu-id="aa7d4-101">Get photo</span></span>

<span data-ttu-id="aa7d4-102">Obtenha a [profilePhoto](../resources/profilephoto.md) especificada ou seus metadados (propriedades de profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="aa7d4-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

<span data-ttu-id="aa7d4-103">Uma operação GET procura a foto especificada na caixa de correio do usuário no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-103">A GET operation looks for the specified photo in the user's mailbox on Exchange Online.</span></span>

> <span data-ttu-id="aa7d4-104">**Observação** Esta operação na versão 1.0 é compatível com caixas de correio corporativas ou de estudante ou caixas de correio não pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="aa7d4-104">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa7d4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa7d4-105">Permissions</span></span>
<span data-ttu-id="aa7d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa7d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

*   <span data-ttu-id="aa7d4-108">Foto do perfil de qualquer usuário no locatário, incluindo o usuário conectado – User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa7d4-108">Profile photo of any user in the tenant including the signed-in user - User.ReadBasic.All; User.Read.All; User.ReadWrite.All</span></span>
*   <span data-ttu-id="aa7d4-109">Foto do perfil especificamente do usuário conectado – User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa7d4-109">Profile photo of specifically the signed-in user - User.Read, User.ReadWrite; User.ReadBasic.All; User.Read.All; User.ReadWrite.All</span></span>
* <span data-ttu-id="aa7d4-110">Foto do perfil de um **grupo** – Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa7d4-110">Profile photo of a **group**Group.Read.All; Group.ReadWrite.All</span></span>
* <span data-ttu-id="aa7d4-111">Foto de um **contato** – Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa7d4-111">Photo of a **contact** - Contacts.Read, Contacts.ReadWrite</span></span>

## <a name="http-request-to-get-the-photo"></a><span data-ttu-id="aa7d4-112">Solicitação HTTP para obter a foto</span><span class="sxs-lookup"><span data-stu-id="aa7d4-112">HTTP request to get the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="http-request-to-get-the-metadata-of-the-photo"></a><span data-ttu-id="aa7d4-113">Solicitação HTTP para obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="aa7d4-113">HTTP request to get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa7d4-114">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa7d4-114">Optional query parameters</span></span>
<span data-ttu-id="aa7d4-115">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-115">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa7d4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa7d4-116">Request headers</span></span>
| <span data-ttu-id="aa7d4-117">Nome</span><span class="sxs-lookup"><span data-stu-id="aa7d4-117">Name</span></span>       | <span data-ttu-id="aa7d4-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa7d4-118">Type</span></span> | <span data-ttu-id="aa7d4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa7d4-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa7d4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa7d4-120">Authorization</span></span>  | <span data-ttu-id="aa7d4-121">string</span><span class="sxs-lookup"><span data-stu-id="aa7d4-121">string</span></span>  | <span data-ttu-id="aa7d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa7d4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa7d4-124">Request body</span></span>
<span data-ttu-id="aa7d4-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-125">Do not supply a request body for this method.</span></span>
## <a name="response-for-getting-the-photo"></a><span data-ttu-id="aa7d4-126">Resposta para obter a foto</span><span class="sxs-lookup"><span data-stu-id="aa7d4-126">Response for getting the photo</span></span>
<span data-ttu-id="aa7d4-p103">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e dados binários da foto solicitada.  Se não existirem fotos, a operação retornará `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-p103">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
## <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="aa7d4-129">Resposta para obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="aa7d4-129">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="aa7d4-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [profilePhoto](../resources/profilePhoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-130">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa7d4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa7d4-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="aa7d4-132">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="aa7d4-132">Request 1</span></span>
<span data-ttu-id="aa7d4-133">Esta solicitação obtém a foto do usuário conectado, com o maior tamanho disponível.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-133">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="aa7d4-134">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="aa7d4-134">Response 1</span></span>
<span data-ttu-id="aa7d4-p104">Contém os dados binários da foto solicitada. O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-p104">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="aa7d4-137">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="aa7d4-137">Request 2</span></span>
<span data-ttu-id="aa7d4-138">Esta solicitação obtém os metadados da foto do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-138">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-2"></a><span data-ttu-id="aa7d4-139">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="aa7d4-139">Response 2</span></span>

<span data-ttu-id="aa7d4-p105">Os dados de resposta a seguir mostram os metadados da foto. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-p105">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="aa7d4-p106">Os dados de resposta a seguir mostram o conteúdo de uma resposta quando uma foto ainda não foi carregada para o usuário. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="aa7d4-p106">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
