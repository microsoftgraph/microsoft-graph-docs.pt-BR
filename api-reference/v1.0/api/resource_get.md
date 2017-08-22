# <a name="get-resource"></a><span data-ttu-id="aa650-101">Obter recurso</span><span class="sxs-lookup"><span data-stu-id="aa650-101">Get resource</span></span>

<span data-ttu-id="aa650-102">Recupere os dados binários do objeto [resource](../resources/resource.md) de um arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="aa650-102">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa650-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa650-103">Prerequisites</span></span>
<span data-ttu-id="aa650-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="aa650-104">One of the following **scopes** is required to execute this API:</span></span>  

<span data-ttu-id="aa650-105">Notes.Read, Notes.ReadWrite, Notes.Read.All ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa650-105">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="aa650-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa650-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="aa650-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa650-107">Request headers</span></span>
| <span data-ttu-id="aa650-108">Nome</span><span class="sxs-lookup"><span data-stu-id="aa650-108">Name</span></span>       | <span data-ttu-id="aa650-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa650-109">Type</span></span> | <span data-ttu-id="aa650-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa650-110">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa650-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa650-111">Authorization</span></span>  | <span data-ttu-id="aa650-112">string</span><span class="sxs-lookup"><span data-stu-id="aa650-112">string</span></span>  | <span data-ttu-id="aa650-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa650-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa650-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa650-115">Request body</span></span>
<span data-ttu-id="aa650-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa650-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa650-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa650-117">Response</span></span>

<span data-ttu-id="aa650-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e os dados binários do arquivo ou imagem no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa650-118">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="aa650-119">Observação: As imagens não serão renderizadas diretamente em um navegador porque elas exigem autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="aa650-119">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="aa650-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa650-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa650-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa650-121">Request</span></span>
<span data-ttu-id="aa650-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa650-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="aa650-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa650-123">Response</span></span>
<span data-ttu-id="aa650-124">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa650-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
