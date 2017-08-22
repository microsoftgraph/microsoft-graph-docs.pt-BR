# <a name="list-names"></a><span data-ttu-id="51f52-101">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="51f52-101">List names</span></span>

<span data-ttu-id="51f52-102">Recupere uma lista de itens nomeados associados à planilha.</span><span class="sxs-lookup"><span data-stu-id="51f52-102">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="51f52-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51f52-103">Prerequisites</span></span>
<span data-ttu-id="51f52-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="51f52-104">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="51f52-105">Files.Read</span><span class="sxs-lookup"><span data-stu-id="51f52-105">Files.Read</span></span>
  * <span data-ttu-id="51f52-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51f52-106">Files.ReadWrite</span></span>
  * <span data-ttu-id="51f52-107">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="51f52-107">Sites.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="51f52-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51f52-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="51f52-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="51f52-109">Optional query parameters</span></span>
<span data-ttu-id="51f52-110">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="51f52-110">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51f52-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51f52-111">Request headers</span></span>
| <span data-ttu-id="51f52-112">Nome</span><span class="sxs-lookup"><span data-stu-id="51f52-112">Name</span></span>      |<span data-ttu-id="51f52-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="51f52-113">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51f52-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="51f52-114">Authorization</span></span>  | <span data-ttu-id="51f52-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51f52-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="51f52-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51f52-117">Request body</span></span>
<span data-ttu-id="51f52-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51f52-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51f52-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f52-119">Response</span></span>

<span data-ttu-id="51f52-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [NamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51f52-120">If successful, this method returns a `200 OK` response code and collection of [NamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51f52-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51f52-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51f52-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51f52-122">Request</span></span>
<span data-ttu-id="51f52-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51f52-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="51f52-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f52-124">Response</span></span>
<span data-ttu-id="51f52-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51f52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
