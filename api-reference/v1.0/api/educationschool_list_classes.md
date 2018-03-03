# <a name="list-educationclasses"></a><span data-ttu-id="09fab-101">Listar educationClasses</span><span class="sxs-lookup"><span data-stu-id="09fab-101">List educationClasses</span></span>

<span data-ttu-id="09fab-102">Recupera uma lista de classes de propriedade de uma escola.</span><span class="sxs-lookup"><span data-stu-id="09fab-102">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="09fab-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="09fab-103">Permissions</span></span>
<span data-ttu-id="09fab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="09fab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="09fab-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09fab-106">Permission type</span></span>      | <span data-ttu-id="09fab-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09fab-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09fab-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09fab-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="09fab-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="09fab-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="09fab-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09fab-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="09fab-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09fab-111">Not supported.</span></span>  |
|<span data-ttu-id="09fab-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09fab-112">Application</span></span> | <span data-ttu-id="09fab-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09fab-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="09fab-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09fab-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09fab-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09fab-115">Optional query parameters</span></span>
<span data-ttu-id="09fab-116">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09fab-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09fab-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09fab-117">Request headers</span></span>
| <span data-ttu-id="09fab-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09fab-118">Header</span></span>       | <span data-ttu-id="09fab-119">Valor</span><span class="sxs-lookup"><span data-stu-id="09fab-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09fab-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="09fab-120">Authorization</span></span>  | <span data-ttu-id="09fab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09fab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09fab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09fab-123">Request body</span></span>
<span data-ttu-id="09fab-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09fab-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="09fab-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="09fab-125">Response</span></span>
<span data-ttu-id="09fab-126">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09fab-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09fab-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09fab-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09fab-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09fab-128">Request</span></span>
<span data-ttu-id="09fab-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="09fab-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/10002/classes
```
##### <a name="response"></a><span data-ttu-id="09fab-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="09fab-130">Response</span></span>
<span data-ttu-id="09fab-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09fab-131">The following is an example of the response.</span></span> 

><span data-ttu-id="09fab-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09fab-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
