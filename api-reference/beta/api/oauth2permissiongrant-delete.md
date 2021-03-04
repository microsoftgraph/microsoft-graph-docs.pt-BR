---
title: Excluir um oAuth2PermissionGrant
description: Exclua um oAuth2PermissionGrant, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: b026f2e254a0901526baddaf786ab8d1d6efab6d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447937"
---
# <a name="delete-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="cd5b8-103">Excluir uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="cd5b8-103">Delete a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="cd5b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd5b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd5b8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd5b8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd5b8-106">Excluir um [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="cd5b8-106">Delete an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="cd5b8-107">Quando uma concessão de permissão delegada é excluída, o acesso concedido é revogado.</span><span class="sxs-lookup"><span data-stu-id="cd5b8-107">When a delegated permission grant is deleted, the access it granted is revoked.</span></span> <span data-ttu-id="cd5b8-108">Tokens de acesso existentes continuarão a ser válidos para sua vida útil, mas novos tokens de acesso não serão concedidos para as permissões delegadas identificadas no **oAuth2PermissionGrant** excluído .</span><span class="sxs-lookup"><span data-stu-id="cd5b8-108">Existing access tokens will continue to be valid for their lifetime, but new access tokens will not be granted for the delegated permissions identified in the deleted **oAuth2PermissionGrant**.</span></span>

> [!NOTE]
> <span data-ttu-id="cd5b8-109">Pode haver duas concessões de permissão delegadas autorizando um aplicativo a agir em nome de um usuário ao chamar uma API.</span><span class="sxs-lookup"><span data-stu-id="cd5b8-109">There may be two delegated permission grants authorizing an application to act on behalf of a user when calling an API.</span></span> <span data-ttu-id="cd5b8-110">Isso pode acontecer quando um usuário consente para o aplicativo em seu próprio nome (criando um **oAuth2PermissionGrant** com **consentType** *Principal*, identificando o usuário) e, em seguida, um administrador concede consentimento de administrador em todo o locatário em nome de todos os usuários (criando um segundo **oAuth2PermissionGrant** com **consentType** de *AllPrincipals*).</span><span class="sxs-lookup"><span data-stu-id="cd5b8-110">This can happen when a user consents for the application on their own behalf (creating an **oAuth2PermissionGrant** with **consentType** *Principal*, identifying the user) and then an administrator grants tenant-wide admin consent on behalf of all users (creating a second **oAuth2PermissionGrant** with **consentType** of *AllPrincipals*).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd5b8-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd5b8-111">Permissions</span></span>

<span data-ttu-id="cd5b8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd5b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd5b8-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd5b8-114">Permission type</span></span>      | <span data-ttu-id="cd5b8-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd5b8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd5b8-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd5b8-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cd5b8-117">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd5b8-117">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd5b8-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd5b8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd5b8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd5b8-119">Not supported.</span></span>    |
|<span data-ttu-id="cd5b8-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd5b8-120">Application</span></span> | <span data-ttu-id="cd5b8-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd5b8-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd5b8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd5b8-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cd5b8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd5b8-123">Request headers</span></span>

| <span data-ttu-id="cd5b8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="cd5b8-124">Name</span></span>       | <span data-ttu-id="cd5b8-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd5b8-125">Type</span></span> | <span data-ttu-id="cd5b8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd5b8-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cd5b8-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd5b8-127">Authorization</span></span>  | <span data-ttu-id="cd5b8-128">string</span><span class="sxs-lookup"><span data-stu-id="cd5b8-128">string</span></span>  | <span data-ttu-id="cd5b8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd5b8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd5b8-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd5b8-131">Request body</span></span>

<span data-ttu-id="cd5b8-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd5b8-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd5b8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd5b8-133">Response</span></span>

<span data-ttu-id="cd5b8-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd5b8-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd5b8-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd5b8-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd5b8-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd5b8-137">Request</span></span>

<span data-ttu-id="cd5b8-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd5b8-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd5b8-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd5b8-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2PermissionGrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="cd5b8-140">C#</span><span class="sxs-lookup"><span data-stu-id="cd5b8-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd5b8-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd5b8-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd5b8-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd5b8-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd5b8-143">Java</span><span class="sxs-lookup"><span data-stu-id="cd5b8-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cd5b8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd5b8-144">Response</span></span>

<span data-ttu-id="cd5b8-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd5b8-145">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


