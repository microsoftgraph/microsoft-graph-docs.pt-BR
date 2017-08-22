# <a name="list-contracts"></a><span data-ttu-id="6777e-101">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="6777e-101">List contracts</span></span>

<span data-ttu-id="6777e-102">Recupere uma lista de objetos [contract](../resources/contract.md) associados a um locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="6777e-102">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6777e-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6777e-103">Prerequisites</span></span>

<span data-ttu-id="6777e-104">Um dos seguintes **scopes** é necessário para executar esta API: *Directory.Read.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="6777e-104">One of the following **scopes** are required to execute this API: *Directory.Read.All*, *Directory.ReadWrite.All*, or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="6777e-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6777e-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6777e-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6777e-106">Optional query parameters</span></span>

<span data-ttu-id="6777e-107">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6777e-107">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="6777e-108">A filtragem é compatível com customerId, defaultDomainName e displayName.</span><span class="sxs-lookup"><span data-stu-id="6777e-108">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6777e-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6777e-109">Request headers</span></span>

| <span data-ttu-id="6777e-110">Nome</span><span class="sxs-lookup"><span data-stu-id="6777e-110">Name</span></span>      |<span data-ttu-id="6777e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6777e-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6777e-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="6777e-112">Authorization</span></span>  | <span data-ttu-id="6777e-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6777e-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6777e-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6777e-115">Request body</span></span>

<span data-ttu-id="6777e-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6777e-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6777e-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="6777e-117">Response</span></span>

<span data-ttu-id="6777e-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6777e-118">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6777e-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6777e-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6777e-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6777e-120">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="6777e-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="6777e-121">Response</span></span>

<span data-ttu-id="6777e-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6777e-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->