# <a name="create-contactfolder"></a><span data-ttu-id="ba33e-101">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="ba33e-101">Create ContactFolder</span></span>

<span data-ttu-id="ba33e-102">Cria uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="ba33e-102">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="ba33e-103">Também é possível [criar uma nova contactFolder sob a pasta de contatos padrão do usuário](user_post_contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="ba33e-103">You can also [create a new contactFolder under the user's default contact folder](user_post_contactfolders.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba33e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba33e-104">Prerequisites</span></span>
<span data-ttu-id="ba33e-105">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="ba33e-105">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="ba33e-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba33e-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="ba33e-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba33e-107">Request headers</span></span>
| <span data-ttu-id="ba33e-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba33e-108">Header</span></span>       | <span data-ttu-id="ba33e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ba33e-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba33e-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba33e-110">Authorization</span></span>  | <span data-ttu-id="ba33e-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba33e-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ba33e-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba33e-113">Content-Type</span></span>  | <span data-ttu-id="ba33e-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba33e-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba33e-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba33e-116">Request body</span></span>
<span data-ttu-id="ba33e-117">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ba33e-117">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ba33e-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba33e-118">Response</span></span>

<span data-ttu-id="ba33e-119">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba33e-119">If successful, this method returns `201, Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba33e-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba33e-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba33e-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba33e-121">Request</span></span>
<span data-ttu-id="ba33e-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba33e-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="ba33e-123">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ba33e-123">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ba33e-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba33e-124">Response</span></span>
<span data-ttu-id="ba33e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba33e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
