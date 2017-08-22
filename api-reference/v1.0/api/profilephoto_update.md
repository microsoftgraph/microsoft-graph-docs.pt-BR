# <a name="update-profilephoto"></a><span data-ttu-id="ffbe1-101">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="ffbe1-101">Update profilephoto</span></span>

<span data-ttu-id="ffbe1-p101">Atualize a foto do **user** conectado, ou do **group** ou **contact** especificado. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-p101">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="ffbe1-104">Você pode usar PATCH ou PUT para esta operação na versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-104">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="ffbe1-105">**Observação** Esta operação na versão 1.0 é compatível com caixas de correio corporativas ou de estudante ou caixas de correio não pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="ffbe1-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="ffbe1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ffbe1-106">Prerequisites</span></span>
<span data-ttu-id="ffbe1-107">Um dos seguintes **escopos** é necessário para executar essa API para:</span><span class="sxs-lookup"><span data-stu-id="ffbe1-107">One of the following **scopes** is required to execute this API for:</span></span>

- <span data-ttu-id="ffbe1-108">Foto do perfil de **usuário** conectado  - *User.ReadWrite*, *User.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="ffbe1-108">Profile photo of the signed-in **user** - *User.ReadWrite*, *User.ReadWrite.All*</span></span>
- <span data-ttu-id="ffbe1-109">Foto do perfil de um **group**  -  *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="ffbe1-109">Profile photo of a **group** - *Group.ReadWrite.All*</span></span>
- <span data-ttu-id="ffbe1-110">Foto de um **contact**  -  *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="ffbe1-110">Photo of a **contact** - *Contacts.ReadWrite*</span></span>

> <span data-ttu-id="ffbe1-p102">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão de aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário. Para saber mais, veja como [obter acesso sem um usuário conectado](../../../concepts/auth_v2_service.md).</span><span class="sxs-lookup"><span data-stu-id="ffbe1-p102">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](../../../concepts/auth_v2_service.md).</span></span>

## <a name="http-request-to-update-the-photo"></a><span data-ttu-id="ffbe1-113">Solicitação HTTP para atualizar a foto</span><span class="sxs-lookup"><span data-stu-id="ffbe1-113">HTTP request to update the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="ffbe1-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffbe1-114">Request headers</span></span>
| <span data-ttu-id="ffbe1-115">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ffbe1-115">Header</span></span>       | <span data-ttu-id="ffbe1-116">Valor</span><span class="sxs-lookup"><span data-stu-id="ffbe1-116">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ffbe1-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffbe1-117">Authorization</span></span>  | <span data-ttu-id="ffbe1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ffbe1-120">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ffbe1-120">Content-Type</span></span>  | <span data-ttu-id="ffbe1-p104">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-p104">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ffbe1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffbe1-123">Request body</span></span>
<span data-ttu-id="ffbe1-124">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-124">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="ffbe1-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffbe1-125">Response</span></span>

<span data-ttu-id="ffbe1-126">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-126">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="ffbe1-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffbe1-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffbe1-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffbe1-128">Request</span></span>
<span data-ttu-id="ffbe1-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="ffbe1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffbe1-130">Response</span></span>
<span data-ttu-id="ffbe1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ffbe1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
