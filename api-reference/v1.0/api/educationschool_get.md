# <a name="get-educationschool"></a><span data-ttu-id="e917f-101">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="e917f-101">Get educationSchool</span></span>

<span data-ttu-id="e917f-102">Recupere as propriedades e relações do objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="e917f-102">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e917f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e917f-103">Permissions</span></span>
<span data-ttu-id="e917f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e917f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e917f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e917f-106">Permission type</span></span>      | <span data-ttu-id="e917f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e917f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e917f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e917f-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="e917f-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e917f-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="e917f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e917f-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e917f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e917f-111">Not supported.</span></span>  |
|<span data-ttu-id="e917f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e917f-112">Application</span></span> | <span data-ttu-id="e917f-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e917f-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e917f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e917f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e917f-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e917f-115">Optional query parameters</span></span>
<span data-ttu-id="e917f-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e917f-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e917f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e917f-117">Request headers</span></span>
| <span data-ttu-id="e917f-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e917f-118">Header</span></span>       | <span data-ttu-id="e917f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e917f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e917f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e917f-120">Authorization</span></span>  | <span data-ttu-id="e917f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e917f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e917f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e917f-123">Request body</span></span>
<span data-ttu-id="e917f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e917f-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e917f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e917f-125">Response</span></span>
<span data-ttu-id="e917f-126">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e917f-126">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e917f-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e917f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e917f-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e917f-128">Request</span></span>
<span data-ttu-id="e917f-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e917f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="e917f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e917f-130">Response</span></span>
<span data-ttu-id="e917f-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e917f-131">The following is an example of the response.</span></span> 

><span data-ttu-id="e917f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e917f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "principalEmail": "AmyRoebuck@contoso.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->