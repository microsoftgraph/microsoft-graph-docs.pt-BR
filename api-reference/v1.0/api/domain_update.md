# <a name="update-domain"></a><span data-ttu-id="9eb17-101">Atualizar domínio</span><span class="sxs-lookup"><span data-stu-id="9eb17-101">Update domain</span></span>

<span data-ttu-id="9eb17-102">Atualize as propriedades do objeto de domínio.</span><span class="sxs-lookup"><span data-stu-id="9eb17-102">Update the properties of domain object.</span></span>

> <span data-ttu-id="9eb17-103">**Importante:** Somente domínios verificados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="9eb17-103">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="9eb17-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="9eb17-104">Permissions</span></span>

<span data-ttu-id="9eb17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9eb17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9eb17-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9eb17-107">Permission type</span></span>      | <span data-ttu-id="9eb17-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9eb17-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9eb17-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9eb17-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9eb17-110">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9eb17-110">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9eb17-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9eb17-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eb17-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9eb17-112">Not supported.</span></span>    |
|<span data-ttu-id="9eb17-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9eb17-113">Application</span></span> | <span data-ttu-id="9eb17-114">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eb17-114">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eb17-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9eb17-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="9eb17-116">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="9eb17-116">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9eb17-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb17-117">Request headers</span></span>

| <span data-ttu-id="9eb17-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9eb17-118">Name</span></span>       | <span data-ttu-id="9eb17-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eb17-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9eb17-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9eb17-120">Authorization</span></span>  | <span data-ttu-id="9eb17-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9eb17-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9eb17-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9eb17-123">Content-Type</span></span>  | <span data-ttu-id="9eb17-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9eb17-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9eb17-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb17-125">Request body</span></span>

<span data-ttu-id="9eb17-p103">No corpo da solicitação, forneça os valores para os campos relevantes que serão atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter melhor desempenho, somente inclua valores alterados.</span><span class="sxs-lookup"><span data-stu-id="9eb17-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="9eb17-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eb17-129">Response</span></span>

<span data-ttu-id="9eb17-130">Se bem-sucedido, este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9eb17-130">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eb17-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9eb17-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9eb17-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9eb17-132">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="9eb17-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9eb17-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->