# <a name="force-domain-deletion"></a><span data-ttu-id="8ea8b-101">Força a exclusão de domínio</span><span class="sxs-lookup"><span data-stu-id="8ea8b-101">Force domain deletion</span></span>

<span data-ttu-id="8ea8b-102">Exclui um domínio usando uma operação de longa execução assíncrona.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-102">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="8ea8b-103">As seguintes ações são executadas como parte dessa operação:</span><span class="sxs-lookup"><span data-stu-id="8ea8b-103">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="8ea8b-104">Atualizações de `userPrincipalName`, `mail`, e `proxyAddresses` propriedades de `users` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-104">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="8ea8b-105">Atualizações de `mail` propriedade do `groups` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-105">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="8ea8b-106">Atualizações de `identifierUris` propriedade do `applications` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-106">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="8ea8b-107">Se o número de objetos a ser renomeado for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-107">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="8ea8b-108">Se um do `applications` a ser renomeado é um aplicativo de multilocatário, será retornado um erro.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-108">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="8ea8b-109">Após a exclusão de domínio for concluído, as operações de API para o domínio excluído retornará um código de status HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-109">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="8ea8b-110">Para verificar a exclusão de um domínio, você pode executar uma operação [obter o domínio](domain_get.md) .</span><span class="sxs-lookup"><span data-stu-id="8ea8b-110">To verify deletion of a domain, you can perform a [get domain](domain_get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ea8b-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="8ea8b-111">Permissions</span></span>

<span data-ttu-id="8ea8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ea8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ea8b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ea8b-114">Permission type</span></span>      | <span data-ttu-id="8ea8b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ea8b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ea8b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ea8b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8ea8b-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ea8b-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ea8b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ea8b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ea8b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-119">Not supported.</span></span>    |
|<span data-ttu-id="8ea8b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ea8b-120">Application</span></span> | <span data-ttu-id="8ea8b-121">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ea8b-121">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ea8b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ea8b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="8ea8b-123">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-123">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ea8b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ea8b-124">Request headers</span></span>

| <span data-ttu-id="8ea8b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="8ea8b-125">Name</span></span> | <span data-ttu-id="8ea8b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ea8b-126">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="8ea8b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ea8b-127">Authorization</span></span>  | <span data-ttu-id="8ea8b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8ea8b-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ea8b-130">Content-Type</span></span>  | <span data-ttu-id="8ea8b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="8ea8b-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ea8b-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ea8b-132">Request body</span></span>

<span data-ttu-id="8ea8b-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ea8b-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8ea8b-134">Parameter</span></span> | <span data-ttu-id="8ea8b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ea8b-135">Type</span></span> | <span data-ttu-id="8ea8b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ea8b-136">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="8ea8b-137">Opção para desabilitar contas de usuário que são renomeadas.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-137">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="8ea8b-138">Se uma conta de usuário estiver desabilitada, o usuário não poderão entrar.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-138">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="8ea8b-139">Se definida como **true** o `users` atualizados como parte dessa operação será desabilitado.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-139">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="8ea8b-140">Valor padrão é **true**.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-140">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="8ea8b-141">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="8ea8b-141">Response body</span></span>

<span data-ttu-id="8ea8b-142">Se tiver êxito, este método retornará `HTTP/1.1 204 OK` código de status.</span><span class="sxs-lookup"><span data-stu-id="8ea8b-142">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="8ea8b-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ea8b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ea8b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ea8b-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a><span data-ttu-id="8ea8b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ea8b-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->