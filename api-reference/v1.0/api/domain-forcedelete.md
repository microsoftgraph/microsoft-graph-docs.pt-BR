---
title: Forçar exclusão de domínio
description: Exclui um domínio usando uma operação assíncrona de execução longa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bbf56fdd2f623a918b43298626bd08269ad922ef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467502"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="43137-103">Forçar exclusão de domínio</span><span class="sxs-lookup"><span data-stu-id="43137-103">Force domain deletion</span></span>

<span data-ttu-id="43137-104">Exclui um domínio usando uma operação assíncrona de execução longa.</span><span class="sxs-lookup"><span data-stu-id="43137-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="43137-105">As ações a seguir são executadas como parte desta operação:</span><span class="sxs-lookup"><span data-stu-id="43137-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="43137-106">atualiza as `userPrincipalName`propriedades `mail`, e `proxyAddresses` de `users` com referências para o domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="43137-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="43137-107">Atualiza a `mail` propriedade de `groups` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="43137-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="43137-108">Atualiza a `identifierUris` propriedade de `applications` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.</span><span class="sxs-lookup"><span data-stu-id="43137-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="43137-109">Se o número de objetos a serem renomeados for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="43137-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="43137-110">Se um dos `applications` a ser renomeado for um aplicativo de vários locatários, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="43137-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="43137-111">Após a conclusão da exclusão do domínio, as operações de API para o domínio excluído retornarão um código de status HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="43137-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="43137-112">Para verificar a exclusão de um domínio, você pode executar uma operação [Get Domain](domain-get.md) .</span><span class="sxs-lookup"><span data-stu-id="43137-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="43137-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="43137-113">Permissions</span></span>

<span data-ttu-id="43137-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43137-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43137-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43137-116">Permission type</span></span>      | <span data-ttu-id="43137-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43137-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43137-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43137-118">Delegated (work or school account)</span></span> | <span data-ttu-id="43137-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43137-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43137-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43137-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43137-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43137-121">Not supported.</span></span>    |
|<span data-ttu-id="43137-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43137-122">Application</span></span> | <span data-ttu-id="43137-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43137-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43137-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43137-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="43137-125">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="43137-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43137-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43137-126">Request headers</span></span>

| <span data-ttu-id="43137-127">Nome</span><span class="sxs-lookup"><span data-stu-id="43137-127">Name</span></span> | <span data-ttu-id="43137-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="43137-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="43137-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="43137-129">Authorization</span></span>  | <span data-ttu-id="43137-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43137-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="43137-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43137-132">Content-Type</span></span>  | <span data-ttu-id="43137-133">application/json</span><span class="sxs-lookup"><span data-stu-id="43137-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="43137-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43137-134">Request body</span></span>

<span data-ttu-id="43137-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43137-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="43137-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="43137-136">Parameter</span></span> | <span data-ttu-id="43137-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="43137-137">Type</span></span> | <span data-ttu-id="43137-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="43137-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="43137-139">Opção para desabilitar as contas de usuário que são renomeadas.</span><span class="sxs-lookup"><span data-stu-id="43137-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="43137-140">Se uma conta de usuário estiver desabilitada, o usuário não terá permissão para entrar.</span><span class="sxs-lookup"><span data-stu-id="43137-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="43137-141">Se definido como **true** , `users` a parte atualizada como parte dessa operação será desabilitada.</span><span class="sxs-lookup"><span data-stu-id="43137-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="43137-142">O valor padrão é **true**.</span><span class="sxs-lookup"><span data-stu-id="43137-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="43137-143">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="43137-143">Response body</span></span>

<span data-ttu-id="43137-144">Se bem-sucedido, este método retorna `HTTP/1.1 204 OK` o código de status.</span><span class="sxs-lookup"><span data-stu-id="43137-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="43137-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43137-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="43137-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43137-146">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="43137-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="43137-147">Response</span></span>

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
