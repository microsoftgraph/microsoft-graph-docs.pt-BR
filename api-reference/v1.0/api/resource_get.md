# <a name="get-resource"></a><span data-ttu-id="55dd6-101">Obter recurso</span><span class="sxs-lookup"><span data-stu-id="55dd6-101">Get resource</span></span>

<span data-ttu-id="55dd6-102">Recupere os dados binários do objeto [resource](../resources/resource.md) de um arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="55dd6-102">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="55dd6-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="55dd6-103">Permissions</span></span>
<span data-ttu-id="55dd6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55dd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55dd6-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55dd6-106">Permission type</span></span>      | <span data-ttu-id="55dd6-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55dd6-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="55dd6-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55dd6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="55dd6-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55dd6-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="55dd6-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55dd6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55dd6-111">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55dd6-111">Notes.Read, Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="55dd6-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55dd6-112">Application</span></span> | <span data-ttu-id="55dd6-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55dd6-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="55dd6-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55dd6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="55dd6-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55dd6-115">Request headers</span></span>
| <span data-ttu-id="55dd6-116">Nome</span><span class="sxs-lookup"><span data-stu-id="55dd6-116">Name</span></span>       | <span data-ttu-id="55dd6-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="55dd6-117">Type</span></span> | <span data-ttu-id="55dd6-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="55dd6-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="55dd6-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="55dd6-119">Authorization</span></span>  | <span data-ttu-id="55dd6-120">string</span><span class="sxs-lookup"><span data-stu-id="55dd6-120">string</span></span>  | <span data-ttu-id="55dd6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55dd6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55dd6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55dd6-123">Request body</span></span>
<span data-ttu-id="55dd6-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55dd6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55dd6-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="55dd6-125">Response</span></span>

<span data-ttu-id="55dd6-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e os dados binários do arquivo ou imagem no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55dd6-126">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="55dd6-127">Observação: As imagens não serão renderizadas diretamente em um navegador porque elas exigem autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="55dd6-127">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="55dd6-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55dd6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55dd6-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55dd6-129">Request</span></span>
<span data-ttu-id="55dd6-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55dd6-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="55dd6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="55dd6-131">Response</span></span>
<span data-ttu-id="55dd6-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55dd6-132">Here is an example of the response.</span></span>
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
