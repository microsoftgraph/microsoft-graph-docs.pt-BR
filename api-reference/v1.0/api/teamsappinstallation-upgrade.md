---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b2ec98883f3db8b8f9ba20b19b6848fc5bd99b5b
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/21/2020
ms.locfileid: "45197048"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="e6fc9-103">Atualizar um aplicativo em uma equipe</span><span class="sxs-lookup"><span data-stu-id="e6fc9-103">Upgrade an app in a team</span></span>

<span data-ttu-id="e6fc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6fc9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6fc9-105">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6fc9-105">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6fc9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6fc9-106">Permissions</span></span>

<span data-ttu-id="e6fc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6fc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6fc9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6fc9-109">Permission type</span></span>      | <span data-ttu-id="e6fc9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6fc9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6fc9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6fc9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e6fc9-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e6fc9-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="e6fc9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6fc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6fc9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6fc9-114">Not supported.</span></span>    |
|<span data-ttu-id="e6fc9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6fc9-115">Application</span></span> | <span data-ttu-id="e6fc9-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e6fc9-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6fc9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6fc9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="e6fc9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6fc9-118">Request headers</span></span>

| <span data-ttu-id="e6fc9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6fc9-119">Header</span></span>       | <span data-ttu-id="e6fc9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e6fc9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6fc9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6fc9-121">Authorization</span></span>  | <span data-ttu-id="e6fc9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6fc9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6fc9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6fc9-124">Request body</span></span>

<span data-ttu-id="e6fc9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6fc9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6fc9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6fc9-126">Response</span></span>

<span data-ttu-id="e6fc9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6fc9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6fc9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6fc9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6fc9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6fc9-130">Request</span></span>

<span data-ttu-id="e6fc9-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6fc9-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6fc9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6fc9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="e6fc9-133">C#</span><span class="sxs-lookup"><span data-stu-id="e6fc9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6fc9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6fc9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6fc9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6fc9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6fc9-136">Java</span><span class="sxs-lookup"><span data-stu-id="e6fc9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e6fc9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6fc9-137">Response</span></span>

<span data-ttu-id="e6fc9-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6fc9-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
