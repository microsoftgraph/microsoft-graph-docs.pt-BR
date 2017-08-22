# <a name="update-domain"></a><span data-ttu-id="2f710-101">Atualizar domínio</span><span class="sxs-lookup"><span data-stu-id="2f710-101">Update domain</span></span>

<span data-ttu-id="2f710-102">Atualize as propriedades do objeto de domínio.</span><span class="sxs-lookup"><span data-stu-id="2f710-102">Update the properties of domain object.</span></span>

> <span data-ttu-id="2f710-103">**Importante:** Somente domínios verificados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="2f710-103">**Important:** Only verified domains can be updated.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f710-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f710-104">Prerequisites</span></span>

<span data-ttu-id="2f710-105">Um dos seguintes **escopos** é obrigatório para executar esta API: *Domain.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="2f710-105">One of the following **scopes** is required to execute this API: *Domain.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="2f710-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f710-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="2f710-107">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="2f710-107">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f710-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f710-108">Request headers</span></span>

| <span data-ttu-id="2f710-109">Nome</span><span class="sxs-lookup"><span data-stu-id="2f710-109">Name</span></span>       | <span data-ttu-id="2f710-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f710-110">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2f710-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f710-111">Authorization</span></span>  | <span data-ttu-id="2f710-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f710-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f710-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f710-114">Content-Type</span></span>  | <span data-ttu-id="2f710-115">application/json</span><span class="sxs-lookup"><span data-stu-id="2f710-115">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f710-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f710-116">Request body</span></span>

<span data-ttu-id="2f710-p102">No corpo da solicitação, forneça os valores para os campos relevantes que serão atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter melhor desempenho, somente inclua valores alterados.</span><span class="sxs-lookup"><span data-stu-id="2f710-p102">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="2f710-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f710-120">Response</span></span>

<span data-ttu-id="2f710-121">Se bem-sucedido, este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f710-121">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f710-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f710-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f710-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f710-123">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/V1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="2f710-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f710-124">Response</span></span>

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