# <a name="create-notebook"></a><span data-ttu-id="6c7ec-101">Criar bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="6c7ec-101">Create notebook</span></span>

<span data-ttu-id="6c7ec-102">Crie um novo [bloco de anotações](../resources/notebook.md) do OneNote.</span><span class="sxs-lookup"><span data-stu-id="6c7ec-102">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6c7ec-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c7ec-103">Permissions</span></span>
<span data-ttu-id="6c7ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6c7ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c7ec-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c7ec-106">Permission type</span></span>      | <span data-ttu-id="6c7ec-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c7ec-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c7ec-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c7ec-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6c7ec-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7ec-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c7ec-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c7ec-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c7ec-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c7ec-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6c7ec-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c7ec-112">Application</span></span> | <span data-ttu-id="6c7ec-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7ec-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c7ec-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c7ec-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="6c7ec-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7ec-115">Request headers</span></span>
| <span data-ttu-id="6c7ec-116">Nome</span><span class="sxs-lookup"><span data-stu-id="6c7ec-116">Name</span></span>       | <span data-ttu-id="6c7ec-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c7ec-117">Type</span></span> | <span data-ttu-id="6c7ec-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c7ec-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c7ec-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c7ec-119">Authorization</span></span>  | <span data-ttu-id="6c7ec-120">string</span><span class="sxs-lookup"><span data-stu-id="6c7ec-120">string</span></span>  | <span data-ttu-id="6c7ec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c7ec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c7ec-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c7ec-123">Content-Type</span></span> | <span data-ttu-id="6c7ec-124">string</span><span class="sxs-lookup"><span data-stu-id="6c7ec-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6c7ec-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7ec-125">Request body</span></span>
<span data-ttu-id="6c7ec-126">No corpo da solicitação, forneça um nome para o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="6c7ec-126">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="6c7ec-p103">Os nomes dos blocos de anotações devem ser exclusivos. O nome não pode conter mais de 128 caracteres ou conter os seguintes caracteres:  ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="6c7ec-p103">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="6c7ec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7ec-129">Response</span></span>

<span data-ttu-id="6c7ec-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c7ec-130">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c7ec-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c7ec-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c7ec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7ec-132">Request</span></span>
<span data-ttu-id="6c7ec-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c7ec-133">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6c7ec-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7ec-134">Response</span></span>
<span data-ttu-id="6c7ec-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c7ec-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
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
