---
title: Forçar exclusão de domínio
description: Exclui um domínio usando uma operação assíncrona de execução longa.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a662d86f3050fdad5e371f0d62c93745fa98afed
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889950"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="e55af-103">Forçar exclusão de domínio</span><span class="sxs-lookup"><span data-stu-id="e55af-103">Force domain deletion</span></span>

<span data-ttu-id="e55af-104">Exclui um domínio usando uma operação assíncrona de execução longa.</span><span class="sxs-lookup"><span data-stu-id="e55af-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="e55af-105">As ações a seguir são executadas como parte desta operação:</span><span class="sxs-lookup"><span data-stu-id="e55af-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="e55af-106">Atualiza as `userPrincipalName`propriedades `mail`, e `proxyAddresses` de `users` com referências para o domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="e55af-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="e55af-107">Atualiza a `mail` propriedade de `groups` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="e55af-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="e55af-108">Atualiza a `identifierUris` propriedade de `applications` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="e55af-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="e55af-109">Se o número de objetos a serem renomeados for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="e55af-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="e55af-110">Se um dos `applications` a ser renomeado for um aplicativo de vários locatários, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="e55af-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="e55af-111">Após a conclusão da exclusão do domínio, as operações de API para o domínio excluído retornarão um código de status HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="e55af-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="e55af-112">Para verificar a exclusão de um domínio, você pode executar uma operação [Get Domain](domain-get.md) .</span><span class="sxs-lookup"><span data-stu-id="e55af-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="e55af-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="e55af-113">Permissions</span></span>

<span data-ttu-id="e55af-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e55af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e55af-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e55af-116">Permission type</span></span>      | <span data-ttu-id="e55af-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e55af-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e55af-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e55af-118">Delegated (work or school account)</span></span> | <span data-ttu-id="e55af-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e55af-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e55af-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e55af-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e55af-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e55af-121">Not supported.</span></span>    |
|<span data-ttu-id="e55af-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e55af-122">Application</span></span> | <span data-ttu-id="e55af-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e55af-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e55af-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e55af-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="e55af-125">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="e55af-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e55af-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e55af-126">Request headers</span></span>

| <span data-ttu-id="e55af-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e55af-127">Name</span></span> | <span data-ttu-id="e55af-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e55af-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e55af-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e55af-129">Authorization</span></span>  | <span data-ttu-id="e55af-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e55af-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e55af-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e55af-132">Content-Type</span></span>  | <span data-ttu-id="e55af-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e55af-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e55af-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e55af-134">Request body</span></span>

<span data-ttu-id="e55af-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e55af-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e55af-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e55af-136">Parameter</span></span> | <span data-ttu-id="e55af-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="e55af-137">Type</span></span> | <span data-ttu-id="e55af-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e55af-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="e55af-139">Opção para desabilitar as contas de usuário que são renomeadas.</span><span class="sxs-lookup"><span data-stu-id="e55af-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="e55af-140">Se uma conta de usuário estiver desabilitada, o usuário não terá permissão para entrar.</span><span class="sxs-lookup"><span data-stu-id="e55af-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="e55af-141">Se definido como **true** , `users` a parte atualizada como parte dessa operação será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="e55af-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="e55af-142">O valor padrão é **true**.</span><span class="sxs-lookup"><span data-stu-id="e55af-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="e55af-143">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="e55af-143">Response body</span></span>

<span data-ttu-id="e55af-144">Se bem-sucedido, este método retorna `HTTP/1.1 204 OK` o código de status.</span><span class="sxs-lookup"><span data-stu-id="e55af-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="e55af-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e55af-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="e55af-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e55af-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e55af-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e55af-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e55af-148">C#</span><span class="sxs-lookup"><span data-stu-id="e55af-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e55af-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="e55af-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e55af-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e55af-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e55af-151">Java</span><span class="sxs-lookup"><span data-stu-id="e55af-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e55af-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e55af-152">Response</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
