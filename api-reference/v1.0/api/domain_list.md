# <a name="list-domains"></a><span data-ttu-id="a06bb-101">Listar domínios</span><span class="sxs-lookup"><span data-stu-id="a06bb-101">List domains</span></span>

<span data-ttu-id="a06bb-102">Recupere uma lista de objetos domain.</span><span class="sxs-lookup"><span data-stu-id="a06bb-102">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a06bb-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a06bb-103">Permissions</span></span>
<span data-ttu-id="a06bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a06bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a06bb-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a06bb-106">Permission type</span></span>      | <span data-ttu-id="a06bb-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a06bb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a06bb-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a06bb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a06bb-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a06bb-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="a06bb-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a06bb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a06bb-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a06bb-111">Not supported.</span></span>    |
|<span data-ttu-id="a06bb-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a06bb-112">Application</span></span> | <span data-ttu-id="a06bb-113">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a06bb-113">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a06bb-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a06bb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a06bb-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a06bb-115">Optional query parameters</span></span>
<span data-ttu-id="a06bb-116">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a06bb-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a06bb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a06bb-117">Request headers</span></span>
| <span data-ttu-id="a06bb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a06bb-118">Name</span></span>      |<span data-ttu-id="a06bb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a06bb-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a06bb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a06bb-120">Authorization</span></span>  | <span data-ttu-id="a06bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a06bb-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a06bb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a06bb-123">Accept</span></span>         | <span data-ttu-id="a06bb-124">application/json;</span><span class="sxs-lookup"><span data-stu-id="a06bb-124">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="a06bb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a06bb-125">Request body</span></span>
<span data-ttu-id="a06bb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a06bb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a06bb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a06bb-127">Response</span></span>

<span data-ttu-id="a06bb-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a06bb-128">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a06bb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a06bb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a06bb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a06bb-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains
```
##### <a name="response"></a><span data-ttu-id="a06bb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a06bb-131">Response</span></span>
<span data-ttu-id="a06bb-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a06bb-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->