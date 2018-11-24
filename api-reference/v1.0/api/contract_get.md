# <a name="get-contract"></a><span data-ttu-id="133fa-101">Obter Contract</span><span class="sxs-lookup"><span data-stu-id="133fa-101">Get Contract</span></span>

<span data-ttu-id="133fa-102">Recupere as propriedades e os relacionamentos do objeto [contract](../resources/contract.md).</span><span class="sxs-lookup"><span data-stu-id="133fa-102">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="133fa-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="133fa-103">Permissions</span></span>

<span data-ttu-id="133fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="133fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="133fa-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="133fa-106">Permission type</span></span>      | <span data-ttu-id="133fa-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="133fa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="133fa-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="133fa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="133fa-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="133fa-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="133fa-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="133fa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="133fa-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="133fa-111">Not supported.</span></span>    |
|<span data-ttu-id="133fa-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="133fa-112">Application</span></span> | <span data-ttu-id="133fa-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="133fa-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="133fa-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="133fa-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="133fa-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="133fa-115">Optional query parameters</span></span>

<span data-ttu-id="133fa-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="133fa-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="133fa-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="133fa-117">Request headers</span></span>

| <span data-ttu-id="133fa-118">Nome</span><span class="sxs-lookup"><span data-stu-id="133fa-118">Name</span></span>      |<span data-ttu-id="133fa-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="133fa-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="133fa-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="133fa-120">Authorization</span></span>  | <span data-ttu-id="133fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="133fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="133fa-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="133fa-123">Request body</span></span>

<span data-ttu-id="133fa-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="133fa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="133fa-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="133fa-125">Response</span></span>

<span data-ttu-id="133fa-126">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="133fa-126">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="133fa-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="133fa-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="133fa-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="133fa-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="133fa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="133fa-129">Response</span></span>
<span data-ttu-id="133fa-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="133fa-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
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