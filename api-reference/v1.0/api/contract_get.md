# <a name="get-contract"></a><span data-ttu-id="9f0bd-101">Obter Contract</span><span class="sxs-lookup"><span data-stu-id="9f0bd-101">Get Contract</span></span>

<span data-ttu-id="9f0bd-102">Recupere as propriedades e os relacionamentos do objeto [contract](../resources/contract.md).</span><span class="sxs-lookup"><span data-stu-id="9f0bd-102">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f0bd-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f0bd-103">Prerequisites</span></span>

<span data-ttu-id="9f0bd-104">Um dos seguintes **scopes** é necessário para executar esta API: *Directory.Read.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="9f0bd-104">One of the following **scopes** are required to execute this API: *Directory.Read.All*, *Directory.ReadWrite.All*, or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="9f0bd-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f0bd-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f0bd-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9f0bd-106">Optional query parameters</span></span>

<span data-ttu-id="9f0bd-107">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9f0bd-107">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f0bd-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f0bd-108">Request headers</span></span>

| <span data-ttu-id="9f0bd-109">Nome</span><span class="sxs-lookup"><span data-stu-id="9f0bd-109">Name</span></span>      |<span data-ttu-id="9f0bd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f0bd-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f0bd-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f0bd-111">Authorization</span></span>  | <span data-ttu-id="9f0bd-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f0bd-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f0bd-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f0bd-114">Request body</span></span>

<span data-ttu-id="9f0bd-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f0bd-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f0bd-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f0bd-116">Response</span></span>

<span data-ttu-id="9f0bd-117">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f0bd-117">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f0bd-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f0bd-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f0bd-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f0bd-119">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="9f0bd-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f0bd-120">Response</span></span>
<span data-ttu-id="9f0bd-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f0bd-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
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