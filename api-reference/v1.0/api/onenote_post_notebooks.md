# <a name="create-notebook"></a><span data-ttu-id="915d1-101">Criar bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="915d1-101">Create notebook</span></span>

<span data-ttu-id="915d1-102">Crie um novo [bloco de anotações](../resources/notebook.md) do OneNote.</span><span class="sxs-lookup"><span data-stu-id="915d1-102">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="915d1-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="915d1-103">Prerequisites</span></span>
<span data-ttu-id="915d1-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="915d1-104">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="915d1-105">Notes.Create, Notes.ReadWrite ou Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="915d1-105">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="915d1-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="915d1-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="915d1-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="915d1-107">Request headers</span></span>
| <span data-ttu-id="915d1-108">Nome</span><span class="sxs-lookup"><span data-stu-id="915d1-108">Name</span></span>       | <span data-ttu-id="915d1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="915d1-109">Type</span></span> | <span data-ttu-id="915d1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="915d1-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="915d1-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="915d1-111">Authorization</span></span>  | <span data-ttu-id="915d1-112">string</span><span class="sxs-lookup"><span data-stu-id="915d1-112">string</span></span>  | <span data-ttu-id="915d1-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="915d1-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="915d1-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="915d1-115">Content-Type</span></span> | <span data-ttu-id="915d1-116">string</span><span class="sxs-lookup"><span data-stu-id="915d1-116">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="915d1-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="915d1-117">Request body</span></span>
<span data-ttu-id="915d1-118">No corpo da solicitação, forneça um nome para o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="915d1-118">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="915d1-p102">Os nomes dos blocos de anotações devem ser exclusivos. O nome não pode conter mais de 128 caracteres ou conter os seguintes caracteres:  ?*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="915d1-p102">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="915d1-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="915d1-121">Response</span></span>

<span data-ttu-id="915d1-122">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="915d1-122">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="915d1-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="915d1-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="915d1-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="915d1-124">Request</span></span>
<span data-ttu-id="915d1-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="915d1-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="915d1-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="915d1-126">Response</span></span>
<span data-ttu-id="915d1-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="915d1-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->