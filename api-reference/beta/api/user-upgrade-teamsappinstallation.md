---
title: 'teamsAppInstallation: atualização'
description: Atualizar uma instalação de aplicativo no escopo pessoal de um usuário
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 906828d4d14bdf19cfd8b2bc5f904e7219b40e55
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/21/2020
ms.locfileid: "45196915"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="77f46-103">teamsAppInstallation: atualização</span><span class="sxs-lookup"><span data-stu-id="77f46-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="77f46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77f46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77f46-105">Atualize uma [instalação de aplicativo](../resources/teamsappinstallation.md) no escopo pessoal do [usuário](../resources/user.md) especificado para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="77f46-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="77f46-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="77f46-106">Permissions</span></span>

<span data-ttu-id="77f46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77f46-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77f46-109">Permission type</span></span>      | <span data-ttu-id="77f46-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77f46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77f46-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77f46-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77f46-112">TeamsAppInstallation. ReadWriteForUser, User. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="77f46-112">TeamsAppInstallation.ReadWriteForUser, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="77f46-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77f46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77f46-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77f46-114">Not supported.</span></span>    |
|<span data-ttu-id="77f46-115">Application</span><span class="sxs-lookup"><span data-stu-id="77f46-115">Application</span></span> | <span data-ttu-id="77f46-116">TeamsAppInstallation. ReadWriteForUser. All, User. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="77f46-116">TeamsAppInstallation.ReadWriteForUser.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77f46-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77f46-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="77f46-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77f46-118">Request headers</span></span>

| <span data-ttu-id="77f46-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77f46-119">Header</span></span>       | <span data-ttu-id="77f46-120">Valor</span><span class="sxs-lookup"><span data-stu-id="77f46-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77f46-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="77f46-121">Authorization</span></span>  | <span data-ttu-id="77f46-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77f46-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77f46-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77f46-124">Request body</span></span>

<span data-ttu-id="77f46-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77f46-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77f46-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="77f46-126">Response</span></span>

<span data-ttu-id="77f46-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77f46-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77f46-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77f46-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="77f46-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77f46-130">Request</span></span>

<span data-ttu-id="77f46-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="77f46-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="77f46-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="77f46-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="77f46-133">C#</span><span class="sxs-lookup"><span data-stu-id="77f46-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77f46-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77f46-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77f46-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77f46-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77f46-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="77f46-136">Response</span></span>

<span data-ttu-id="77f46-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="77f46-137">The following is an example of the response.</span></span>

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
