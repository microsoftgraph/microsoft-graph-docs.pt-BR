# <a name="update-page"></a><span data-ttu-id="193c7-101">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="193c7-101">Update page</span></span>

<span data-ttu-id="193c7-102">Atualize o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="193c7-102">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="193c7-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="193c7-103">Permissions</span></span>
<span data-ttu-id="193c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="193c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="193c7-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="193c7-106">Permission type</span></span>      | <span data-ttu-id="193c7-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="193c7-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="193c7-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="193c7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="193c7-109">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="193c7-109">Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="193c7-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="193c7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="193c7-111">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="193c7-111">Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="193c7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="193c7-112">Application</span></span> | <span data-ttu-id="193c7-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="193c7-113">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="193c7-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="193c7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="193c7-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="193c7-115">Request headers</span></span>
| <span data-ttu-id="193c7-116">Nome</span><span class="sxs-lookup"><span data-stu-id="193c7-116">Name</span></span>       | <span data-ttu-id="193c7-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="193c7-117">Type</span></span> | <span data-ttu-id="193c7-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="193c7-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="193c7-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="193c7-119">Authorization</span></span>  | <span data-ttu-id="193c7-120">string</span><span class="sxs-lookup"><span data-stu-id="193c7-120">string</span></span>  | <span data-ttu-id="193c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="193c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="193c7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="193c7-123">Content-Type</span></span> | <span data-ttu-id="193c7-124">string</span><span class="sxs-lookup"><span data-stu-id="193c7-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="193c7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="193c7-125">Request body</span></span>
<span data-ttu-id="193c7-p103">No corpo da solicitação, forneça uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representa as alterações da página. Veja mais informações e exemplos em <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Atualizar páginas do OneNote</a>.</span><span class="sxs-lookup"><span data-stu-id="193c7-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="193c7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="193c7-128">Response</span></span>

<span data-ttu-id="193c7-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.  Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="193c7-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="193c7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="193c7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="193c7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="193c7-132">Request</span></span>
<span data-ttu-id="193c7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="193c7-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="193c7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="193c7-134">Response</span></span>
<span data-ttu-id="193c7-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="193c7-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
