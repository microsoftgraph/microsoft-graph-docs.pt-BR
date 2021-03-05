---
title: Forçar a exclusão de domínio
description: Exclui um domínio usando uma operação de longa execução assíncrona.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a4376961ea843c5c512d5bdf59449a7e765399f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441974"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="c7a85-103">Forçar a exclusão de domínio</span><span class="sxs-lookup"><span data-stu-id="c7a85-103">Force domain deletion</span></span>

<span data-ttu-id="c7a85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7a85-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7a85-105">Exclui um domínio usando uma operação de longa execução assíncrona.</span><span class="sxs-lookup"><span data-stu-id="c7a85-105">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="c7a85-106">Antes de chamar [forceDelete,](domain-forcedelete.md)você deve atualizar ou remover quaisquer referências ao **Exchange** como o serviço de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="c7a85-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="c7a85-107">As seguintes ações são executadas como parte desta operação:</span><span class="sxs-lookup"><span data-stu-id="c7a85-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="c7a85-108">Atualiza as propriedades , e de com referências ao domínio excluído para usar o `userPrincipalName` `mail` domínio onmicrosoft.com `proxyAddresses` `users` inicial.</span><span class="sxs-lookup"><span data-stu-id="c7a85-108">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="c7a85-109">Atualiza a propriedade de com referências ao domínio excluído para usar o `mail` `groups` domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="c7a85-109">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="c7a85-110">Atualiza a propriedade de com referências ao domínio excluído para usar o `identifierUris` `applications` domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="c7a85-110">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="c7a85-111">Se o número de objetos a serem renomeados for maior do que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="c7a85-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="c7a85-112">Se um dos a `applications` ser renomeado for um aplicativo de vários locatários, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="c7a85-112">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="c7a85-113">Após a conclusão da exclusão de domínio, as operações de API para o domínio excluído retornarão um código de status HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="c7a85-113">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="c7a85-114">Para verificar a exclusão de um domínio, você pode executar uma [operação obter domínio.](domain-get.md)</span><span class="sxs-lookup"><span data-stu-id="c7a85-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7a85-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7a85-115">Permissions</span></span>

<span data-ttu-id="c7a85-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7a85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7a85-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7a85-118">Permission type</span></span>      | <span data-ttu-id="c7a85-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7a85-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7a85-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7a85-120">Delegated (work or school account)</span></span> | <span data-ttu-id="c7a85-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c7a85-121">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c7a85-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7a85-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7a85-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7a85-123">Not supported.</span></span>    |
|<span data-ttu-id="c7a85-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7a85-124">Application</span></span> | <span data-ttu-id="c7a85-125">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7a85-125">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7a85-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7a85-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="c7a85-127">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="c7a85-127">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7a85-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a85-128">Request headers</span></span>

| <span data-ttu-id="c7a85-129">Nome</span><span class="sxs-lookup"><span data-stu-id="c7a85-129">Name</span></span> | <span data-ttu-id="c7a85-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a85-130">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c7a85-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7a85-131">Authorization</span></span>  | <span data-ttu-id="c7a85-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7a85-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c7a85-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7a85-134">Content-Type</span></span>  | <span data-ttu-id="c7a85-135">application/json</span><span class="sxs-lookup"><span data-stu-id="c7a85-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7a85-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a85-136">Request body</span></span>

<span data-ttu-id="c7a85-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7a85-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c7a85-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c7a85-138">Parameter</span></span> | <span data-ttu-id="c7a85-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7a85-139">Type</span></span> | <span data-ttu-id="c7a85-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a85-140">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="c7a85-141">Opção para desabilitar contas de usuário renomeadas.</span><span class="sxs-lookup"><span data-stu-id="c7a85-141">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="c7a85-142">Se uma conta de usuário estiver desabilitada, o usuário não poderá entrar.</span><span class="sxs-lookup"><span data-stu-id="c7a85-142">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="c7a85-143">Se definido como **true,** `users` a atualização como parte dessa operação será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="c7a85-143">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="c7a85-144">O valor padrão é **true**.</span><span class="sxs-lookup"><span data-stu-id="c7a85-144">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="c7a85-145">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="c7a85-145">Response body</span></span>

<span data-ttu-id="c7a85-146">Se tiver êxito, este método retornará `HTTP/1.1 204 OK` o código de status.</span><span class="sxs-lookup"><span data-stu-id="c7a85-146">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="c7a85-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7a85-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7a85-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a85-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c7a85-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7a85-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/v1.0/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[<span data-ttu-id="c7a85-150">C#</span><span class="sxs-lookup"><span data-stu-id="c7a85-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7a85-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7a85-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7a85-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7a85-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7a85-153">Java</span><span class="sxs-lookup"><span data-stu-id="c7a85-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7a85-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a85-154">Response</span></span>

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

