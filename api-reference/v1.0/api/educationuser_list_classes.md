# <a name="list-classes"></a><span data-ttu-id="9e5db-101">Listar classes</span><span class="sxs-lookup"><span data-stu-id="9e5db-101">List classes</span></span>

<span data-ttu-id="9e5db-102">Recupere uma lista de objetos de classe.</span><span class="sxs-lookup"><span data-stu-id="9e5db-102">Retrieve a list of chartpoints objects.</span></span> <span data-ttu-id="9e5db-103">Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas.</span><span class="sxs-lookup"><span data-stu-id="9e5db-103">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="9e5db-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e5db-104">Permissions</span></span>
<span data-ttu-id="9e5db-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9e5db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9e5db-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e5db-107">Permission type</span></span>      | <span data-ttu-id="9e5db-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e5db-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e5db-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e5db-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="9e5db-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="9e5db-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="9e5db-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e5db-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9e5db-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e5db-112">Not supported.</span></span>  |
|<span data-ttu-id="9e5db-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e5db-113">Application</span></span> | <span data-ttu-id="9e5db-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e5db-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9e5db-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e5db-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e5db-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e5db-116">Optional query parameters</span></span>
<span data-ttu-id="9e5db-117">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e5db-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e5db-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e5db-118">Request headers</span></span>
| <span data-ttu-id="9e5db-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e5db-119">Header</span></span>       | <span data-ttu-id="9e5db-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9e5db-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e5db-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e5db-121">Authorization</span></span>  | <span data-ttu-id="9e5db-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e5db-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e5db-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e5db-124">Request body</span></span>
<span data-ttu-id="9e5db-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e5db-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9e5db-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e5db-126">Response</span></span>
<span data-ttu-id="9e5db-127">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e5db-127">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e5db-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e5db-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e5db-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e5db-129">Request</span></span>
<span data-ttu-id="9e5db-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e5db-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="9e5db-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e5db-131">Response</span></span>
<span data-ttu-id="9e5db-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e5db-132">The following is an example of the response.</span></span> 

><span data-ttu-id="9e5db-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e5db-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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