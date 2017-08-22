# <a name="delete-domain"></a><span data-ttu-id="4c73f-101">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="4c73f-101">Delete domain</span></span>

<span data-ttu-id="4c73f-102">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="4c73f-102">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="4c73f-103">**Importante:**</span><span class="sxs-lookup"><span data-stu-id="4c73f-103">**Important:**</span></span>
> - <span data-ttu-id="4c73f-104">Os domínios excluídos não podem ser recuperados.</span><span class="sxs-lookup"><span data-stu-id="4c73f-104">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="4c73f-p101">As tentativas de exclusão falharão se houver objetos ou recursos dependentes no domínio. Você pode encontrar todos os recursos dependentes usando a API [Listar domainNameReferences](domain_list_domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="4c73f-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain_list_domainnamereferences.md) API.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c73f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c73f-107">Prerequisites</span></span>

<span data-ttu-id="4c73f-108">Um dos seguintes **escopos** é obrigatório para executar esta API: *Domain.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="4c73f-108">One of the following **scopes** is required to execute this API: *Domain.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="4c73f-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c73f-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="4c73f-110">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="4c73f-110">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c73f-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c73f-111">Request headers</span></span>

| <span data-ttu-id="4c73f-112">Nome</span><span class="sxs-lookup"><span data-stu-id="4c73f-112">Name</span></span>       | <span data-ttu-id="4c73f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c73f-113">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4c73f-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c73f-114">Authorization</span></span>  | <span data-ttu-id="4c73f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c73f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c73f-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c73f-117">Content-Type</span></span>  | <span data-ttu-id="4c73f-118">application/json</span><span class="sxs-lookup"><span data-stu-id="4c73f-118">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c73f-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c73f-119">Request body</span></span>

<span data-ttu-id="4c73f-120">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c73f-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c73f-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c73f-121">Response</span></span>

<span data-ttu-id="4c73f-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c73f-p103">If successful, this method returns `204, No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c73f-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c73f-124">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c73f-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c73f-125">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/V1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="4c73f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c73f-126">Response</span></span>

<span data-ttu-id="4c73f-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c73f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->