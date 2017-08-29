# <a name="get-domain"></a><span data-ttu-id="7def8-101">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="7def8-101">Get domain</span></span>

<span data-ttu-id="7def8-102">Recupere as propriedades e os relacionamentos do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="7def8-102">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7def8-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7def8-103">Permissions</span></span>

<span data-ttu-id="7def8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7def8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7def8-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7def8-106">Permission type</span></span>      | <span data-ttu-id="7def8-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7def8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7def8-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7def8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7def8-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7def8-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="7def8-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7def8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7def8-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7def8-111">Not supported.</span></span>    |
|<span data-ttu-id="7def8-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7def8-112">Application</span></span> | <span data-ttu-id="7def8-113">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7def8-113">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7def8-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7def8-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="7def8-115">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="7def8-115">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7def8-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7def8-116">Optional query parameters</span></span>

<span data-ttu-id="7def8-117">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7def8-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7def8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7def8-118">Request headers</span></span>

| <span data-ttu-id="7def8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7def8-119">Name</span></span>      |<span data-ttu-id="7def8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7def8-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7def8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7def8-121">Authorization</span></span>  | <span data-ttu-id="7def8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7def8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7def8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7def8-124">Content-Type</span></span>  | <span data-ttu-id="7def8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7def8-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7def8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7def8-126">Request body</span></span>
<span data-ttu-id="7def8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7def8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7def8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7def8-128">Response</span></span>

<span data-ttu-id="7def8-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7def8-129">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7def8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7def8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7def8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7def8-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="7def8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7def8-132">Response</span></span>
<span data-ttu-id="7def8-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7def8-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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