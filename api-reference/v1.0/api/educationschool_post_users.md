# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="9ab6b-101">Adicionar educationUser a uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="9ab6b-101">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="9ab6b-102">Adicione um usuário a uma escola.</span><span class="sxs-lookup"><span data-stu-id="9ab6b-102">Add a user to a role</span></span>

## <a name="permissions"></a><span data-ttu-id="9ab6b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ab6b-103">Permissions</span></span>
<span data-ttu-id="9ab6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ab6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ab6b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ab6b-106">Permission type</span></span>      | <span data-ttu-id="9ab6b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ab6b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ab6b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ab6b-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ab6b-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab6b-109">Not supported.</span></span>  |
|<span data-ttu-id="9ab6b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ab6b-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ab6b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab6b-111">Not supported.</span></span>  |
|<span data-ttu-id="9ab6b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ab6b-112">Application</span></span> | <span data-ttu-id="9ab6b-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ab6b-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9ab6b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab6b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9ab6b-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab6b-115">Request headers</span></span>
| <span data-ttu-id="9ab6b-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ab6b-116">Header</span></span>       | <span data-ttu-id="9ab6b-117">Valor</span><span class="sxs-lookup"><span data-stu-id="9ab6b-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ab6b-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ab6b-118">Authorization</span></span>  | <span data-ttu-id="9ab6b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ab6b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ab6b-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ab6b-121">Content-Type</span></span>  | <span data-ttu-id="9ab6b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9ab6b-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ab6b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab6b-123">Request body</span></span>
<span data-ttu-id="9ab6b-124">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="9ab6b-124">In the request body, supply a JSON representation of an [invitation](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9ab6b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab6b-125">Response</span></span>
<span data-ttu-id="9ab6b-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ab6b-126">If successful, this method returns a `204 No Content` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ab6b-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ab6b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ab6b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab6b-128">Request</span></span>
<span data-ttu-id="9ab6b-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ab6b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/<id>/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="9ab6b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab6b-130">Response</span></span>
<span data-ttu-id="9ab6b-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ab6b-131">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->