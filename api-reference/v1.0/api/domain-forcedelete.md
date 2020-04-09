---
title: Forçar exclusão de domínio
description: Exclui um domínio usando uma operação assíncrona de execução longa.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b50957082fe4f2e1e0a87d24cf36a7a7fc6eed16
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181340"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="745c6-103">Forçar exclusão de domínio</span><span class="sxs-lookup"><span data-stu-id="745c6-103">Force domain deletion</span></span>

<span data-ttu-id="745c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="745c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="745c6-105">Exclui um domínio usando uma operação assíncrona de execução longa.</span><span class="sxs-lookup"><span data-stu-id="745c6-105">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="745c6-106">As ações a seguir são executadas como parte desta operação:</span><span class="sxs-lookup"><span data-stu-id="745c6-106">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="745c6-107">Atualiza as `userPrincipalName`propriedades `mail`, e `proxyAddresses` de `users` com referências para o domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="745c6-107">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="745c6-108">Atualiza a `mail` propriedade de `groups` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="745c6-108">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="745c6-109">Atualiza a `identifierUris` propriedade de `applications` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="745c6-109">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="745c6-110">Se o número de objetos a serem renomeados for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="745c6-110">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="745c6-111">Se um dos `applications` a ser renomeado for um aplicativo de vários locatários, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="745c6-111">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="745c6-112">Após a conclusão da exclusão do domínio, as operações de API para o domínio excluído retornarão um código de status HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="745c6-112">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="745c6-113">Para verificar a exclusão de um domínio, você pode executar uma operação [Get Domain](domain-get.md) .</span><span class="sxs-lookup"><span data-stu-id="745c6-113">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="745c6-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="745c6-114">Permissions</span></span>

<span data-ttu-id="745c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="745c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="745c6-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="745c6-117">Permission type</span></span>      | <span data-ttu-id="745c6-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="745c6-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="745c6-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="745c6-119">Delegated (work or school account)</span></span> | <span data-ttu-id="745c6-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="745c6-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="745c6-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="745c6-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="745c6-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="745c6-122">Not supported.</span></span>    |
|<span data-ttu-id="745c6-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="745c6-123">Application</span></span> | <span data-ttu-id="745c6-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="745c6-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="745c6-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="745c6-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="745c6-126">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="745c6-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="745c6-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="745c6-127">Request headers</span></span>

| <span data-ttu-id="745c6-128">Nome</span><span class="sxs-lookup"><span data-stu-id="745c6-128">Name</span></span> | <span data-ttu-id="745c6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="745c6-129">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="745c6-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="745c6-130">Authorization</span></span>  | <span data-ttu-id="745c6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="745c6-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="745c6-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="745c6-133">Content-Type</span></span>  | <span data-ttu-id="745c6-134">application/json</span><span class="sxs-lookup"><span data-stu-id="745c6-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="745c6-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="745c6-135">Request body</span></span>

<span data-ttu-id="745c6-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="745c6-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="745c6-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="745c6-137">Parameter</span></span> | <span data-ttu-id="745c6-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="745c6-138">Type</span></span> | <span data-ttu-id="745c6-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="745c6-139">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="745c6-140">Opção para desabilitar as contas de usuário que são renomeadas.</span><span class="sxs-lookup"><span data-stu-id="745c6-140">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="745c6-141">Se uma conta de usuário estiver desabilitada, o usuário não terá permissão para entrar.</span><span class="sxs-lookup"><span data-stu-id="745c6-141">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="745c6-142">Se definido como **true** , `users` a parte atualizada como parte dessa operação será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="745c6-142">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="745c6-143">O valor padrão é **true**.</span><span class="sxs-lookup"><span data-stu-id="745c6-143">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="745c6-144">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="745c6-144">Response body</span></span>

<span data-ttu-id="745c6-145">Se bem-sucedido, este método retorna `HTTP/1.1 204 OK` o código de status.</span><span class="sxs-lookup"><span data-stu-id="745c6-145">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="745c6-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="745c6-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="745c6-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="745c6-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="745c6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="745c6-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="745c6-149">C#</span><span class="sxs-lookup"><span data-stu-id="745c6-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="745c6-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="745c6-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="745c6-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="745c6-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="745c6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="745c6-152">Response</span></span>

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
