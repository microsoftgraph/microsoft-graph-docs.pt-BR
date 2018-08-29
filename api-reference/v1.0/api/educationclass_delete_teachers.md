# <a name="remove-teacher"></a><span data-ttu-id="fdd30-101">Remover professor</span><span class="sxs-lookup"><span data-stu-id="fdd30-101">Remove teacher</span></span>

<span data-ttu-id="fdd30-102">Remova um professor de uma aula.</span><span class="sxs-lookup"><span data-stu-id="fdd30-102">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdd30-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdd30-103">Permissions</span></span>
<span data-ttu-id="fdd30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fdd30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fdd30-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdd30-106">Permission type</span></span>      | <span data-ttu-id="fdd30-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdd30-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdd30-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdd30-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="fdd30-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdd30-109">Not supported.</span></span>  |
|<span data-ttu-id="fdd30-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdd30-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fdd30-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdd30-111">Not supported.</span></span>  |
|<span data-ttu-id="fdd30-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdd30-112">Application</span></span> | <span data-ttu-id="fdd30-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd30-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fdd30-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdd30-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fdd30-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdd30-115">Request headers</span></span>
| <span data-ttu-id="fdd30-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdd30-116">Header</span></span>       | <span data-ttu-id="fdd30-117">Valor</span><span class="sxs-lookup"><span data-stu-id="fdd30-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fdd30-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdd30-118">Authorization</span></span>  | <span data-ttu-id="fdd30-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdd30-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fdd30-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdd30-121">Request body</span></span>
<span data-ttu-id="fdd30-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdd30-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fdd30-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdd30-123">Response</span></span>
<span data-ttu-id="fdd30-124">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="fdd30-124">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdd30-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdd30-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fdd30-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdd30-126">Request</span></span>
<span data-ttu-id="fdd30-127">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdd30-127">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```

##### <a name="response"></a><span data-ttu-id="fdd30-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdd30-128">Response</span></span>
<span data-ttu-id="fdd30-129">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fdd30-129">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
