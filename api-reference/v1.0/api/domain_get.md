# <a name="get-domain"></a><span data-ttu-id="a3363-101">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="a3363-101">Get domain</span></span>

<span data-ttu-id="a3363-102">Recupere as propriedades e os relacionamentos do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="a3363-102">Retrieve the properties and relationships of domain object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3363-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3363-103">Prerequisites</span></span>

<span data-ttu-id="a3363-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All* ou *Domain.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="a3363-104">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Domain.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="a3363-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3363-105">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="a3363-106">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="a3363-106">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a3363-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a3363-107">Optional query parameters</span></span>

<span data-ttu-id="a3363-108">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a3363-108">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3363-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3363-109">Request headers</span></span>

| <span data-ttu-id="a3363-110">Nome</span><span class="sxs-lookup"><span data-stu-id="a3363-110">Name</span></span>      |<span data-ttu-id="a3363-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3363-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3363-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3363-112">Authorization</span></span>  | <span data-ttu-id="a3363-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3363-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3363-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3363-115">Content-Type</span></span>  | <span data-ttu-id="a3363-116">application/json</span><span class="sxs-lookup"><span data-stu-id="a3363-116">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3363-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3363-117">Request body</span></span>
<span data-ttu-id="a3363-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3363-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3363-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3363-119">Response</span></span>

<span data-ttu-id="a3363-120">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3363-120">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a3363-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3363-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3363-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3363-122">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="a3363-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3363-123">Response</span></span>
<span data-ttu-id="a3363-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3363-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->