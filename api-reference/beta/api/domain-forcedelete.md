---
title: 'domínio: forceDelete'
description: Exclui um domínio usando uma operação assíncrona.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f440d9872df9ab61a86e28ea27d14aff112c1538
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956045"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="6b193-103">domínio: forceDelete</span><span class="sxs-lookup"><span data-stu-id="6b193-103">domain: forceDelete</span></span>

<span data-ttu-id="6b193-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b193-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b193-105">Exclui um domínio usando uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="6b193-105">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="6b193-106">As ações a seguir são executadas como parte desta operação:</span><span class="sxs-lookup"><span data-stu-id="6b193-106">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="6b193-107">Renomeia o UPN, o EmailAddress e o ProxyAddress de usuários com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="6b193-107">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="6b193-108">Renomeia o EmailAddress de grupos com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="6b193-108">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="6b193-109">Renomeia a Identifieruris agora de aplicativos com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="6b193-109">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="6b193-110">Se o número de objetos a serem renomeados for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="6b193-110">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="6b193-111">Se um dos aplicativos a ser renomeado for um aplicativo de vários locatários, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="6b193-111">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="6b193-112">Após a conclusão da exclusão do domínio, as operações de API para o domínio excluído retornarão um código de resposta HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="6b193-112">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="6b193-113">Para verificar a exclusão de um domínio, você pode executar um [domínio Get](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="6b193-113">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="6b193-114">Se o domínio tiver sido excluído com êxito, um código de resposta HTTP 404 será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="6b193-114">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b193-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b193-115">Permissions</span></span>

<span data-ttu-id="6b193-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b193-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6b193-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b193-118">Permission type</span></span>      | <span data-ttu-id="6b193-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b193-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b193-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b193-120">Delegated (work or school account)</span></span> | <span data-ttu-id="6b193-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6b193-121">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6b193-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b193-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b193-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b193-123">Not supported.</span></span>    |
|<span data-ttu-id="6b193-124">Application</span><span class="sxs-lookup"><span data-stu-id="6b193-124">Application</span></span> | <span data-ttu-id="6b193-125">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b193-125">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b193-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b193-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="6b193-127">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="6b193-127">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b193-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b193-128">Request headers</span></span>

| <span data-ttu-id="6b193-129">Nome</span><span class="sxs-lookup"><span data-stu-id="6b193-129">Name</span></span>       | <span data-ttu-id="6b193-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b193-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6b193-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b193-131">Authorization</span></span>  | <span data-ttu-id="6b193-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b193-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="6b193-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b193-134">Content-Type</span></span>  | <span data-ttu-id="6b193-135">application/json</span><span class="sxs-lookup"><span data-stu-id="6b193-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b193-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b193-136">Request body</span></span>

<span data-ttu-id="6b193-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b193-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6b193-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6b193-138">Parameter</span></span>    | <span data-ttu-id="6b193-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b193-139">Type</span></span>   |<span data-ttu-id="6b193-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b193-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b193-141">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="6b193-141">disableUserAccounts</span></span>|<span data-ttu-id="6b193-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b193-142">Boolean</span></span>| <span data-ttu-id="6b193-143">Opção para desabilitar contas de usuário renomeadas.</span><span class="sxs-lookup"><span data-stu-id="6b193-143">Option to disable renamed user accounts.</span></span> <span data-ttu-id="6b193-144">Se uma conta de usuário estiver desabilitada, o usuário não terá permissão para entrar.</span><span class="sxs-lookup"><span data-stu-id="6b193-144">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="6b193-145">*True* (padrão): as contas de usuário renomeadas como parte desta operação estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="6b193-145">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="6b193-146">*False* -as contas de usuário renomeadas como parte dessa operação não estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="6b193-146">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="6b193-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b193-147">Response</span></span>

<span data-ttu-id="6b193-148">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="6b193-148">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="6b193-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b193-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b193-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b193-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6b193-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b193-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6b193-152">C#</span><span class="sxs-lookup"><span data-stu-id="6b193-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b193-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b193-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b193-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b193-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b193-155">Java</span><span class="sxs-lookup"><span data-stu-id="6b193-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6b193-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b193-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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


