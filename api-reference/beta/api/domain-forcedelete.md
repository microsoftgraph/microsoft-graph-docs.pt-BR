---
title: 'domain: forceDelete'
description: Exclui um domínio usando uma operação assíncrona.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 47f81a25fc29f6a7eb0bb79c0f4d84e37825183a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786822"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="f6bdf-103">domain: forceDelete</span><span class="sxs-lookup"><span data-stu-id="f6bdf-103">domain: forceDelete</span></span>

<span data-ttu-id="f6bdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6bdf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6bdf-105">Exclui um domínio usando uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-105">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="f6bdf-106">Antes de chamar [forceDelete](domain-forcedelete.md), você deve atualizar ou remover quaisquer referências **Exchange** como o serviço de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="f6bdf-107">As seguintes ações são executadas como parte desta operação:</span><span class="sxs-lookup"><span data-stu-id="f6bdf-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="f6bdf-108">Renomeia o UPN, EmailAddress e ProxyAddress de usuários com referências ao domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="f6bdf-109">Renomeia o EmailAddress de grupos com referências ao domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="f6bdf-110">Renomeia os identificadores de aplicativos com referências ao domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="f6bdf-111">Se o número de objetos a serem renomeados for maior que 1.000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-111">If the number of objects to be renamed is greater than 1,000, an error is returned.</span></span>

* <span data-ttu-id="f6bdf-112">Se um dos aplicativos a ser renomeado for um aplicativo de vários locatários, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="f6bdf-113">Depois que a exclusão de domínio for concluída, as operações de API do domínio excluído retornarão um código de resposta HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="f6bdf-114">Para verificar a exclusão de um domínio, você pode executar um [domínio get](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="f6bdf-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="f6bdf-115">Se o domínio foi excluído com êxito, um código de resposta HTTP 404 será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6bdf-116">Permissions</span><span class="sxs-lookup"><span data-stu-id="f6bdf-116">Permissions</span></span>

<span data-ttu-id="f6bdf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6bdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f6bdf-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6bdf-119">Permission type</span></span>      | <span data-ttu-id="f6bdf-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6bdf-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6bdf-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6bdf-121">Delegated (work or school account)</span></span> | <span data-ttu-id="f6bdf-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6bdf-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6bdf-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6bdf-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6bdf-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-124">Not supported.</span></span>    |
|<span data-ttu-id="f6bdf-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6bdf-125">Application</span></span> | <span data-ttu-id="f6bdf-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bdf-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6bdf-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6bdf-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="f6bdf-128">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6bdf-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bdf-129">Request headers</span></span>

| <span data-ttu-id="f6bdf-130">Nome</span><span class="sxs-lookup"><span data-stu-id="f6bdf-130">Name</span></span>       | <span data-ttu-id="f6bdf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6bdf-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f6bdf-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6bdf-132">Authorization</span></span>  | <span data-ttu-id="f6bdf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f6bdf-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6bdf-135">Content-Type</span></span>  | <span data-ttu-id="f6bdf-136">application/json</span><span class="sxs-lookup"><span data-stu-id="f6bdf-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6bdf-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bdf-137">Request body</span></span>

<span data-ttu-id="f6bdf-138">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f6bdf-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f6bdf-139">Parameter</span></span>    | <span data-ttu-id="f6bdf-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6bdf-140">Type</span></span>   |<span data-ttu-id="f6bdf-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6bdf-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6bdf-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="f6bdf-142">disableUserAccounts</span></span>|<span data-ttu-id="f6bdf-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6bdf-143">Boolean</span></span>| <span data-ttu-id="f6bdf-144">Opção para desabilitar contas de usuário renomeadas.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="f6bdf-145">Se uma conta de usuário estiver desabilitada, o usuário não poderá entrar.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="f6bdf-146">*True* (padrão) - As contas de usuário renomeadas como parte dessa operação estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="f6bdf-147">*False* - As contas de usuário renomeadas como parte dessa operação não estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="f6bdf-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6bdf-148">Response</span></span>

<span data-ttu-id="f6bdf-149">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f6bdf-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="f6bdf-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6bdf-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6bdf-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bdf-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6bdf-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6bdf-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[<span data-ttu-id="f6bdf-153">C#</span><span class="sxs-lookup"><span data-stu-id="f6bdf-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6bdf-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6bdf-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6bdf-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6bdf-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6bdf-156">Java</span><span class="sxs-lookup"><span data-stu-id="f6bdf-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f6bdf-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6bdf-157">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


