---
title: 'domínio: forceDelete'
description: Exclui um domínio usando uma operação assíncrona.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99ea7666050ba167503fe330bd1c4b9b48aff64b
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655765"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="bf6cb-103">domínio: forceDelete</span><span class="sxs-lookup"><span data-stu-id="bf6cb-103">domain: forceDelete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf6cb-104">Exclui um domínio usando uma operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-104">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="bf6cb-105">As ações a seguir são executadas como parte desta operação:</span><span class="sxs-lookup"><span data-stu-id="bf6cb-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="bf6cb-106">Renomeia o UPN, o EmailAddress e o ProxyAddress de usuários com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-106">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="bf6cb-107">Renomeia o EmailAddress de grupos com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-107">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="bf6cb-108">Renomeia a Identifieruris agora de aplicativos com referências para o domínio excluído.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-108">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="bf6cb-109">Se o número de objetos a serem renomeados for maior que 1000, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="bf6cb-110">Se um dos aplicativos a ser renomeado for um aplicativo de vários locatários, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-110">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="bf6cb-111">Após a conclusão da exclusão do domínio, as operações de API para o domínio excluído retornarão um código de resposta HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-111">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="bf6cb-112">Para verificar a exclusão de um domínio, você pode executar um [domínio Get](domain-get.md).</span><span class="sxs-lookup"><span data-stu-id="bf6cb-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="bf6cb-113">Se o domínio tiver sido excluído com êxito, um código de resposta HTTP 404 será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-113">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf6cb-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf6cb-114">Permissions</span></span>

<span data-ttu-id="bf6cb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf6cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bf6cb-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf6cb-117">Permission type</span></span>      | <span data-ttu-id="bf6cb-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf6cb-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf6cb-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf6cb-119">Delegated (work or school account)</span></span> | <span data-ttu-id="bf6cb-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf6cb-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf6cb-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf6cb-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf6cb-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-122">Not supported.</span></span>    |
|<span data-ttu-id="bf6cb-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf6cb-123">Application</span></span> | <span data-ttu-id="bf6cb-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf6cb-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf6cb-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6cb-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="bf6cb-126">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf6cb-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf6cb-127">Request headers</span></span>

| <span data-ttu-id="bf6cb-128">Nome</span><span class="sxs-lookup"><span data-stu-id="bf6cb-128">Name</span></span>       | <span data-ttu-id="bf6cb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf6cb-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bf6cb-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf6cb-130">Authorization</span></span>  | <span data-ttu-id="bf6cb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="bf6cb-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf6cb-133">Content-Type</span></span>  | <span data-ttu-id="bf6cb-134">application/json</span><span class="sxs-lookup"><span data-stu-id="bf6cb-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf6cb-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf6cb-135">Request body</span></span>

<span data-ttu-id="bf6cb-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bf6cb-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bf6cb-137">Parameter</span></span>    | <span data-ttu-id="bf6cb-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf6cb-138">Type</span></span>   |<span data-ttu-id="bf6cb-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf6cb-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf6cb-140">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="bf6cb-140">disableUserAccounts</span></span>|<span data-ttu-id="bf6cb-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6cb-141">Boolean</span></span>| <span data-ttu-id="bf6cb-142">Opção para desabilitar contas de usuário renomeadas.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-142">Option to disable renamed user accounts.</span></span> <span data-ttu-id="bf6cb-143">Se uma conta de usuário estiver desabilitada, o usuário não terá permissão para entrar.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-143">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="bf6cb-144">*True* (padrão)-as contas de usuário renomeadas como parte dessa operação estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-144">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="bf6cb-145">*False* -as contas de usuário renomeadas como parte dessa operação não estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-145">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="bf6cb-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf6cb-146">Response</span></span>

<span data-ttu-id="bf6cb-147">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="bf6cb-147">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="bf6cb-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf6cb-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf6cb-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf6cb-149">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="bf6cb-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf6cb-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bf6cb-151">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bf6cb-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bf6cb-152">C#</span><span class="sxs-lookup"><span data-stu-id="bf6cb-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf6cb-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="bf6cb-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
