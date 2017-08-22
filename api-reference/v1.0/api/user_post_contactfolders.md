# <a name="create-contactfolder"></a><span data-ttu-id="c9f8a-101">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="c9f8a-101">Create ContactFolder</span></span>

<span data-ttu-id="c9f8a-102">Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9f8a-102">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="c9f8a-103">Você também pode [criar uma nova contactfolder como um filho de qualquer pasta de contatos especificada](contactfolder_post_childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="c9f8a-103">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder_post_childfolders.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9f8a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9f8a-104">Prerequisites</span></span>
<span data-ttu-id="c9f8a-105">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="c9f8a-105">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="c9f8a-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9f8a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="c9f8a-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f8a-107">Request headers</span></span>
| <span data-ttu-id="c9f8a-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9f8a-108">Header</span></span>       | <span data-ttu-id="c9f8a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c9f8a-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9f8a-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9f8a-110">Authorization</span></span>  | <span data-ttu-id="c9f8a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9f8a-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c9f8a-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9f8a-113">Content-Type</span></span>  | <span data-ttu-id="c9f8a-114">application/json</span><span class="sxs-lookup"><span data-stu-id="c9f8a-114">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9f8a-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f8a-115">Request body</span></span>
<span data-ttu-id="c9f8a-116">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c9f8a-116">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c9f8a-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9f8a-117">Response</span></span>

<span data-ttu-id="c9f8a-118">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9f8a-118">If successful, this method returns `201, Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9f8a-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9f8a-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9f8a-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f8a-120">Request</span></span>
<span data-ttu-id="c9f8a-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9f8a-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="c9f8a-122">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c9f8a-122">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c9f8a-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9f8a-123">Response</span></span>
<span data-ttu-id="c9f8a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9f8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
