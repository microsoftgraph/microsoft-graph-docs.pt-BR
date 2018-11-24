# <a name="list-organization"></a><span data-ttu-id="bb88b-101">Listar organização</span><span class="sxs-lookup"><span data-stu-id="bb88b-101">List organization</span></span>



<span data-ttu-id="bb88b-102">Recupere uma lista de objetos de organização.</span><span class="sxs-lookup"><span data-stu-id="bb88b-102">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb88b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb88b-103">Permissions</span></span>
<span data-ttu-id="bb88b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb88b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bb88b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb88b-106">Permission type</span></span>      | <span data-ttu-id="bb88b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb88b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb88b-108">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb88b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bb88b-109">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb88b-109">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="bb88b-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb88b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb88b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb88b-111">Not supported.</span></span>    |
|<span data-ttu-id="bb88b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb88b-112">Application</span></span> | <span data-ttu-id="bb88b-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb88b-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="bb88b-114">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="bb88b-114">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="bb88b-115">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="bb88b-115">All other properties will return with `null` values.</span></span> <span data-ttu-id="bb88b-116">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="bb88b-116">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="bb88b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb88b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb88b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb88b-118">Optional query parameters</span></span>
<span data-ttu-id="bb88b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb88b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bb88b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb88b-120">Request headers</span></span>
| <span data-ttu-id="bb88b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bb88b-121">Name</span></span>       | <span data-ttu-id="bb88b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb88b-122">Type</span></span> | <span data-ttu-id="bb88b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb88b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb88b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb88b-124">Authorization</span></span>  | <span data-ttu-id="bb88b-125">string</span><span class="sxs-lookup"><span data-stu-id="bb88b-125">string</span></span>  | <span data-ttu-id="bb88b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb88b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb88b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb88b-128">Request body</span></span>
<span data-ttu-id="bb88b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb88b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb88b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb88b-130">Response</span></span>

<span data-ttu-id="bb88b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb88b-131">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb88b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb88b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb88b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb88b-133">Request</span></span>
<span data-ttu-id="bb88b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb88b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="bb88b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb88b-135">Response</span></span>
<span data-ttu-id="bb88b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb88b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->