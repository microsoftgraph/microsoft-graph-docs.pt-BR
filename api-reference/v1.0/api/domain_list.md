# <a name="list-domains"></a><span data-ttu-id="0258f-101">Listar domínios</span><span class="sxs-lookup"><span data-stu-id="0258f-101">List domains</span></span>

<span data-ttu-id="0258f-102">Recupere uma lista de objetos domain.</span><span class="sxs-lookup"><span data-stu-id="0258f-102">Retrieve a list of domain objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0258f-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0258f-103">Prerequisites</span></span>
<span data-ttu-id="0258f-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All* ou *Domain.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="0258f-104">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Domain.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="0258f-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0258f-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0258f-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0258f-106">Optional query parameters</span></span>
<span data-ttu-id="0258f-107">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0258f-107">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0258f-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0258f-108">Request headers</span></span>
| <span data-ttu-id="0258f-109">Nome</span><span class="sxs-lookup"><span data-stu-id="0258f-109">Name</span></span>      |<span data-ttu-id="0258f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0258f-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0258f-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="0258f-111">Authorization</span></span>  | <span data-ttu-id="0258f-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0258f-p101">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0258f-114">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0258f-114">Accept</span></span>         | <span data-ttu-id="0258f-115">application/json;</span><span class="sxs-lookup"><span data-stu-id="0258f-115">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="0258f-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0258f-116">Request body</span></span>
<span data-ttu-id="0258f-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0258f-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0258f-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="0258f-118">Response</span></span>

<span data-ttu-id="0258f-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0258f-119">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0258f-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0258f-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0258f-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0258f-121">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains
```
##### <a name="response"></a><span data-ttu-id="0258f-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="0258f-122">Response</span></span>
<span data-ttu-id="0258f-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0258f-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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