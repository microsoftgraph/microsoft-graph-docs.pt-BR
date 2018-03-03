# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="08a37-101">Adicionar educationClass a educationSchool</span><span class="sxs-lookup"><span data-stu-id="08a37-101">Add educationClass to educationSchool</span></span>

<span data-ttu-id="08a37-102">Adicione uma aula a uma escola.</span><span class="sxs-lookup"><span data-stu-id="08a37-102">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="08a37-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="08a37-103">Permissions</span></span>
<span data-ttu-id="08a37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="08a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="08a37-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08a37-106">Permission type</span></span>      | <span data-ttu-id="08a37-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08a37-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08a37-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08a37-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="08a37-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08a37-109">Not supported.</span></span>  |
|<span data-ttu-id="08a37-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08a37-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="08a37-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08a37-111">Not supported.</span></span>  |
|<span data-ttu-id="08a37-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08a37-112">Application</span></span> | <span data-ttu-id="08a37-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a37-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="08a37-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08a37-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="08a37-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08a37-115">Request headers</span></span>
| <span data-ttu-id="08a37-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08a37-116">Header</span></span>       | <span data-ttu-id="08a37-117">Valor</span><span class="sxs-lookup"><span data-stu-id="08a37-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08a37-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="08a37-118">Authorization</span></span>  | <span data-ttu-id="08a37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a37-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="08a37-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08a37-121">Content-Type</span></span>  | <span data-ttu-id="08a37-122">application/json</span><span class="sxs-lookup"><span data-stu-id="08a37-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08a37-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08a37-123">Request body</span></span>
<span data-ttu-id="08a37-124">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="08a37-124">In the request body, supply a JSON representation of an [invitation](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="08a37-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a37-125">Response</span></span>
<span data-ttu-id="08a37-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08a37-126">If successful, this method returns a `204 No Content` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08a37-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08a37-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08a37-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08a37-128">Request</span></span>
<span data-ttu-id="08a37-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08a37-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/v1.0/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="08a37-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a37-130">Response</span></span> 
<span data-ttu-id="08a37-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08a37-131">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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