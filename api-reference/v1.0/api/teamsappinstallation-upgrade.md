---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8525ae7afa33f34d3630a8b5fbac53b3d89dedbc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027276"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="03bba-103">Atualizar um aplicativo em uma equipe</span><span class="sxs-lookup"><span data-stu-id="03bba-103">Upgrade an app in a team</span></span>

<span data-ttu-id="03bba-104">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="03bba-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="03bba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="03bba-105">Permissions</span></span>

<span data-ttu-id="03bba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03bba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03bba-108">Permission type</span></span>      | <span data-ttu-id="03bba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03bba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03bba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03bba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03bba-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03bba-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="03bba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03bba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03bba-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03bba-113">Not supported.</span></span>    |
|<span data-ttu-id="03bba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03bba-114">Application</span></span> | <span data-ttu-id="03bba-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03bba-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="03bba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03bba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="03bba-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03bba-117">Request headers</span></span>

| <span data-ttu-id="03bba-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03bba-118">Header</span></span>       | <span data-ttu-id="03bba-119">Valor</span><span class="sxs-lookup"><span data-stu-id="03bba-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="03bba-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="03bba-120">Authorization</span></span>  | <span data-ttu-id="03bba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03bba-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03bba-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03bba-123">Request body</span></span>

<span data-ttu-id="03bba-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03bba-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03bba-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="03bba-125">Response</span></span>

<span data-ttu-id="03bba-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03bba-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03bba-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03bba-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="03bba-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03bba-129">Request</span></span>

<span data-ttu-id="03bba-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="03bba-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="03bba-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="03bba-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="03bba-132">C#</span><span class="sxs-lookup"><span data-stu-id="03bba-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03bba-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="03bba-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03bba-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="03bba-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="03bba-135">Java</span><span class="sxs-lookup"><span data-stu-id="03bba-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="03bba-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="03bba-136">Response</span></span>

<span data-ttu-id="03bba-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="03bba-137">The following is an example of the response.</span></span> 

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
