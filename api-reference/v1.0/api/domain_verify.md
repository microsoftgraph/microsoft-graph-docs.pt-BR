# <a name="domain-verify"></a><span data-ttu-id="b4971-101">domain: verify</span><span class="sxs-lookup"><span data-stu-id="b4971-101">domain: verify</span></span>

<span data-ttu-id="b4971-102">Valida a propriedade do domínio.</span><span class="sxs-lookup"><span data-stu-id="b4971-102">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="b4971-p101">**Importante:** Aplica-se somente a um domínio não verificado. Para um domínio não verificado, a propriedade isVerified do [domínio](../resources/domain.md) é falsa.</span><span class="sxs-lookup"><span data-stu-id="b4971-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4971-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4971-105">Prerequisites</span></span>

<span data-ttu-id="b4971-106">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All* ou *Domain.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="b4971-106">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Domain.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="b4971-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4971-107">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="b4971-108">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="b4971-108">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4971-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4971-109">Request headers</span></span>

| <span data-ttu-id="b4971-110">Nome</span><span class="sxs-lookup"><span data-stu-id="b4971-110">Name</span></span>       | <span data-ttu-id="b4971-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4971-111">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b4971-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4971-112">Authorization</span></span>  | <span data-ttu-id="b4971-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4971-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b4971-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4971-115">Content-Type</span></span>  | <span data-ttu-id="b4971-116">application/json</span><span class="sxs-lookup"><span data-stu-id="b4971-116">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4971-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4971-117">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b4971-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4971-118">Response</span></span>

<span data-ttu-id="b4971-119">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4971-119">If successful, this method returns `200, OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4971-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4971-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4971-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4971-121">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="b4971-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4971-122">Response</span></span>
<span data-ttu-id="b4971-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4971-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->