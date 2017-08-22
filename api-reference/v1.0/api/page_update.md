# <a name="update-page"></a><span data-ttu-id="38e10-101">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="38e10-101">Update page</span></span>

<span data-ttu-id="38e10-102">Atualize o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="38e10-102">Update the content of a OneNote page.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38e10-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38e10-103">Prerequisites</span></span>
<span data-ttu-id="38e10-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="38e10-104">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="38e10-105">Notes.ReadWrite ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38e10-105">Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="38e10-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38e10-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="38e10-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38e10-107">Request headers</span></span>
| <span data-ttu-id="38e10-108">Nome</span><span class="sxs-lookup"><span data-stu-id="38e10-108">Name</span></span>       | <span data-ttu-id="38e10-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="38e10-109">Type</span></span> | <span data-ttu-id="38e10-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="38e10-110">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="38e10-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="38e10-111">Authorization</span></span>  | <span data-ttu-id="38e10-112">string</span><span class="sxs-lookup"><span data-stu-id="38e10-112">string</span></span>  | <span data-ttu-id="38e10-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38e10-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38e10-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38e10-115">Content-Type</span></span> | <span data-ttu-id="38e10-116">string</span><span class="sxs-lookup"><span data-stu-id="38e10-116">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="38e10-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38e10-117">Request body</span></span>
<span data-ttu-id="38e10-p102">No corpo da solicitação, forneça uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representa as alterações da página. Veja mais informações e exemplos em <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Atualizar páginas do OneNote</a>.</span><span class="sxs-lookup"><span data-stu-id="38e10-p102">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="38e10-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="38e10-120">Response</span></span>

<span data-ttu-id="38e10-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.  Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="38e10-p103">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="38e10-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38e10-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38e10-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38e10-124">Request</span></span>
<span data-ttu-id="38e10-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38e10-125">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="38e10-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="38e10-126">Response</span></span>
<span data-ttu-id="38e10-127">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38e10-127">Here is an example of the response.</span></span> 
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
