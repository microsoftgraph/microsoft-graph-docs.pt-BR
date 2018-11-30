---
title: Força a exclusão de domínio
description: Exclui um domínio usando uma operação de longa execução assíncrona.
ms.openlocfilehash: 20f00679998070b95af65292cadf83d76aa2add1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007358"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="3922e-103">Força a exclusão de domínio</span><span class="sxs-lookup"><span data-stu-id="3922e-103">Force domain deletion</span></span>

<span data-ttu-id="3922e-104">Exclui um domínio usando uma operação de longa execução assíncrona.</span><span class="sxs-lookup"><span data-stu-id="3922e-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="3922e-105">As seguintes ações são executadas como parte dessa operação:</span><span class="sxs-lookup"><span data-stu-id="3922e-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="3922e-106">Atualizações de `userPrincipalName`, `mail`, e `proxyAddresses` propriedades de `users` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="3922e-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="3922e-107">Atualizações de `mail` propriedade do `groups` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="3922e-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="3922e-108">Atualizações de `identifierUris` propriedade do `applications` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="3922e-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="3922e-109">Se o número de objetos a ser renomeado for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="3922e-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="3922e-110">Se um do `applications` a ser renomeado é um aplicativo de multilocatário, será retornado um erro.</span><span class="sxs-lookup"><span data-stu-id="3922e-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="3922e-111">Após a exclusão de domínio for concluído, as operações de API para o domínio excluído retornará um código de status HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="3922e-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="3922e-112">Para verificar a exclusão de um domínio, você pode executar uma operação [obter o domínio](domain-get.md) .</span><span class="sxs-lookup"><span data-stu-id="3922e-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="3922e-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="3922e-113">Permissions</span></span>

<span data-ttu-id="3922e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3922e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3922e-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3922e-116">Permission type</span></span>      | <span data-ttu-id="3922e-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3922e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3922e-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3922e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="3922e-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3922e-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3922e-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3922e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3922e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3922e-121">Not supported.</span></span>    |
|<span data-ttu-id="3922e-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3922e-122">Application</span></span> | <span data-ttu-id="3922e-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3922e-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3922e-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3922e-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="3922e-125">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="3922e-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3922e-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3922e-126">Request headers</span></span>

| <span data-ttu-id="3922e-127">Nome</span><span class="sxs-lookup"><span data-stu-id="3922e-127">Name</span></span> | <span data-ttu-id="3922e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3922e-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3922e-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="3922e-129">Authorization</span></span>  | <span data-ttu-id="3922e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3922e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3922e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3922e-132">Content-Type</span></span>  | <span data-ttu-id="3922e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3922e-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3922e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3922e-134">Request body</span></span>

<span data-ttu-id="3922e-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3922e-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3922e-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3922e-136">Parameter</span></span> | <span data-ttu-id="3922e-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="3922e-137">Type</span></span> | <span data-ttu-id="3922e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="3922e-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="3922e-139">Opção para desabilitar contas de usuário que são renomeadas.</span><span class="sxs-lookup"><span data-stu-id="3922e-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="3922e-140">Se uma conta de usuário estiver desabilitada, o usuário não poderão entrar.</span><span class="sxs-lookup"><span data-stu-id="3922e-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="3922e-141">Se definida como **true** o `users` atualizados como parte dessa operação será desabilitado.</span><span class="sxs-lookup"><span data-stu-id="3922e-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="3922e-142">Valor padrão é **true**.</span><span class="sxs-lookup"><span data-stu-id="3922e-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="3922e-143">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="3922e-143">Response body</span></span>

<span data-ttu-id="3922e-144">Se tiver êxito, este método retornará `HTTP/1.1 204 OK` código de status.</span><span class="sxs-lookup"><span data-stu-id="3922e-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="3922e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3922e-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="3922e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3922e-146">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="3922e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="3922e-147">Response</span></span>

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