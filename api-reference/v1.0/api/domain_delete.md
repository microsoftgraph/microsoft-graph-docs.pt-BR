# <a name="delete-domain"></a><span data-ttu-id="4a864-101">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="4a864-101">Delete domain</span></span>

<span data-ttu-id="4a864-102">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="4a864-102">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="4a864-103">**Importante:**</span><span class="sxs-lookup"><span data-stu-id="4a864-103">**Important:**</span></span>
> - <span data-ttu-id="4a864-104">Os domínios excluídos não podem ser recuperados.</span><span class="sxs-lookup"><span data-stu-id="4a864-104">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="4a864-p101">As tentativas de exclusão falharão se houver objetos ou recursos dependentes no domínio. Você pode encontrar todos os recursos dependentes usando a API [Listar domainNameReferences](domain_list_domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="4a864-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain_list_domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a864-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a864-107">Permissions</span></span>

<span data-ttu-id="4a864-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a864-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4a864-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a864-110">Permission type</span></span>      | <span data-ttu-id="4a864-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a864-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a864-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a864-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a864-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a864-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a864-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a864-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a864-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a864-115">Not supported.</span></span>    |
|<span data-ttu-id="4a864-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a864-116">Application</span></span> | <span data-ttu-id="4a864-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a864-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a864-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a864-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="4a864-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="4a864-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a864-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a864-120">Request headers</span></span>

| <span data-ttu-id="4a864-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4a864-121">Name</span></span>       | <span data-ttu-id="4a864-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a864-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a864-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a864-123">Authorization</span></span>  | <span data-ttu-id="4a864-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a864-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a864-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a864-126">Content-Type</span></span>  | <span data-ttu-id="4a864-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4a864-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a864-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a864-128">Request body</span></span>

<span data-ttu-id="4a864-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a864-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a864-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a864-130">Response</span></span>

<span data-ttu-id="4a864-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a864-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a864-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a864-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a864-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a864-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/V1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="4a864-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a864-135">Response</span></span>

<span data-ttu-id="4a864-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a864-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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