# <a name="domain-verify"></a><span data-ttu-id="0fe2f-101">domain: verify</span><span class="sxs-lookup"><span data-stu-id="0fe2f-101">domain: verify</span></span>

<span data-ttu-id="0fe2f-102">Valida a propriedade do domínio.</span><span class="sxs-lookup"><span data-stu-id="0fe2f-102">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="0fe2f-p101">**Importante:** Aplica-se somente a um domínio não verificado. Para um domínio não verificado, a propriedade isVerified do [domínio](../resources/domain.md) é falsa.</span><span class="sxs-lookup"><span data-stu-id="0fe2f-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fe2f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fe2f-105">Permissions</span></span>

<span data-ttu-id="0fe2f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0fe2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="0fe2f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fe2f-108">Permission type</span></span>      | <span data-ttu-id="0fe2f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fe2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fe2f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fe2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0fe2f-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fe2f-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="0fe2f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fe2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fe2f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fe2f-113">Not supported.</span></span>    |
|<span data-ttu-id="0fe2f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fe2f-114">Application</span></span> | <span data-ttu-id="0fe2f-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe2f-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fe2f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe2f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="0fe2f-117">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="0fe2f-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fe2f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe2f-118">Request headers</span></span>

| <span data-ttu-id="0fe2f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0fe2f-119">Name</span></span>       | <span data-ttu-id="0fe2f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fe2f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0fe2f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fe2f-121">Authorization</span></span>  | <span data-ttu-id="0fe2f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fe2f-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="0fe2f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fe2f-124">Content-Type</span></span>  | <span data-ttu-id="0fe2f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0fe2f-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fe2f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe2f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0fe2f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe2f-127">Response</span></span>

<span data-ttu-id="0fe2f-128">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe2f-128">If successful, this method returns `200, OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fe2f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fe2f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fe2f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe2f-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="0fe2f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe2f-131">Response</span></span>
<span data-ttu-id="0fe2f-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0fe2f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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