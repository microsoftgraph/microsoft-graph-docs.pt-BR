---
title: 'teamsAppInstallation: upgrade'
description: Atualizar uma instalação de aplicativo no escopo pessoal de um usuário
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1dd9a390203658a2f7f284023a05ed0e166e5839
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696272"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="a3836-103">teamsAppInstallation: upgrade</span><span class="sxs-lookup"><span data-stu-id="a3836-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="a3836-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3836-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3836-105">Atualize [uma instalação de](../resources/teamsappinstallation.md) aplicativo no escopo pessoal do usuário [especificado](../resources/user.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a3836-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3836-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3836-106">Permissions</span></span>

<span data-ttu-id="a3836-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3836-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3836-109">Permission type</span></span>      | <span data-ttu-id="a3836-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3836-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3836-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3836-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3836-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="a3836-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="a3836-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3836-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3836-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3836-114">Not supported.</span></span>    |
|<span data-ttu-id="a3836-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3836-115">Application</span></span> | <span data-ttu-id="a3836-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="a3836-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3836-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3836-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id | user-principal-name}/teamwork/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="a3836-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3836-118">Request headers</span></span>

| <span data-ttu-id="a3836-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3836-119">Header</span></span>       | <span data-ttu-id="a3836-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a3836-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3836-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3836-121">Authorization</span></span>  | <span data-ttu-id="a3836-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3836-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3836-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3836-124">Request body</span></span>

<span data-ttu-id="a3836-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3836-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3836-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3836-126">Response</span></span>

<span data-ttu-id="a3836-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3836-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3836-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3836-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3836-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3836-130">Request</span></span>

<span data-ttu-id="a3836-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3836-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a3836-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3836-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk/upgrade
```
# <a name="c"></a>[<span data-ttu-id="a3836-133">C#</span><span class="sxs-lookup"><span data-stu-id="a3836-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3836-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3836-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3836-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3836-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3836-136">Java</span><span class="sxs-lookup"><span data-stu-id="a3836-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3836-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3836-137">Response</span></span>

<span data-ttu-id="a3836-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3836-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "user_upgrade_teamsApp",
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
  "description": "Upgrade teamsApp for user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


