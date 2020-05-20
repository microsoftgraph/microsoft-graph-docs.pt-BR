---
title: Excluir um oAuth2PermissionGrant
description: Excluir um oAuth2PermissionGrant, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bc36f62d1bb0568fc24b48061e427c404f16e43c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288645"
---
# <a name="delete-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="1291a-103">Excluir uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="1291a-103">Delete a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="1291a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1291a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1291a-105">Excluir um [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="1291a-105">Delete an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="1291a-106">Quando uma concessão de permissão delegada é excluída, o acesso concedido é revogado.</span><span class="sxs-lookup"><span data-stu-id="1291a-106">When a delegated permission grant is deleted, the access it granted is revoked.</span></span> <span data-ttu-id="1291a-107">Os tokens de acesso existentes continuarão válidos por seu tempo de vida, mas novos tokens de acesso não serão concedidos para as permissões delegadas identificadas no **oAuth2PermissionGrant**excluído.</span><span class="sxs-lookup"><span data-stu-id="1291a-107">Existing access tokens will continue to be valid for their lifetime, but new access tokens will not be granted for the delegated permissions identified in the deleted **oAuth2PermissionGrant**.</span></span>

> [!NOTE]
> <span data-ttu-id="1291a-108">Pode haver duas permissões delegadas que autorizam um aplicativo a atuar em nome de um usuário ao chamar uma API.</span><span class="sxs-lookup"><span data-stu-id="1291a-108">There may be two delegated permission grants authorizing an application to act on behalf of a user when calling an API.</span></span> <span data-ttu-id="1291a-109">Isso pode acontecer quando um usuário concorda com o aplicativo em seu próprio nome (criando um **oAuth2PermissionGrant** com o **consenttype** *principal*, identificando o usuário) e, em seguida, um administrador concede consentimento de administrador em todo o locatário em nome de todos os usuários (criando um segundo **oAuth2PermissionGrant** com **consenttype** de *servicePrincipalName*).</span><span class="sxs-lookup"><span data-stu-id="1291a-109">This can happen when a user consents for the application on their own behalf (creating an **oAuth2PermissionGrant** with **consentType** *Principal*, identifying the user) and then an administrator grants tenant-wide admin consent on behalf of all users (creating a second **oAuth2PermissionGrant** with **consentType** of *AllPrincipals*).</span></span>

## <a name="permissions"></a><span data-ttu-id="1291a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="1291a-110">Permissions</span></span>

<span data-ttu-id="1291a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1291a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1291a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1291a-113">Permission type</span></span>      | <span data-ttu-id="1291a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1291a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1291a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1291a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1291a-116">DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="1291a-116">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1291a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1291a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1291a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1291a-118">Not supported.</span></span>    |
|<span data-ttu-id="1291a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1291a-119">Application</span></span> | <span data-ttu-id="1291a-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1291a-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1291a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1291a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /oAuth2Permissiongrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1291a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1291a-122">Request headers</span></span>

| <span data-ttu-id="1291a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1291a-123">Name</span></span>       | <span data-ttu-id="1291a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1291a-124">Type</span></span> | <span data-ttu-id="1291a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1291a-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1291a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1291a-126">Authorization</span></span>  | <span data-ttu-id="1291a-127">string</span><span class="sxs-lookup"><span data-stu-id="1291a-127">string</span></span>  | <span data-ttu-id="1291a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1291a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1291a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1291a-130">Request body</span></span>

<span data-ttu-id="1291a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1291a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1291a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1291a-132">Response</span></span>

<span data-ttu-id="1291a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1291a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1291a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1291a-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="1291a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1291a-136">Request</span></span>

<span data-ttu-id="1291a-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1291a-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1291a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1291a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2PermissionGrant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
```

### <a name="response"></a><span data-ttu-id="1291a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1291a-139">Response</span></span>

<span data-ttu-id="1291a-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1291a-140">Here is an example of the response.</span></span>

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
