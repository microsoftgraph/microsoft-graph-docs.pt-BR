---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 69698bf588b6aec789720a7cc1d46a114a5e0621
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421299"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="17e9e-103">Atualizar um aplicativo em uma equipe</span><span class="sxs-lookup"><span data-stu-id="17e9e-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17e9e-104">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17e9e-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="17e9e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="17e9e-105">Permissions</span></span>

<span data-ttu-id="17e9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17e9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17e9e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17e9e-108">Permission type</span></span>      | <span data-ttu-id="17e9e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17e9e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17e9e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17e9e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17e9e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17e9e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="17e9e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17e9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17e9e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17e9e-113">Not supported.</span></span>    |
|<span data-ttu-id="17e9e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17e9e-114">Application</span></span> | <span data-ttu-id="17e9e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17e9e-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17e9e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17e9e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="17e9e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17e9e-117">Request headers</span></span>

| <span data-ttu-id="17e9e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17e9e-118">Header</span></span>       | <span data-ttu-id="17e9e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="17e9e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="17e9e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="17e9e-120">Authorization</span></span>  | <span data-ttu-id="17e9e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17e9e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17e9e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17e9e-123">Request body</span></span>

<span data-ttu-id="17e9e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17e9e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17e9e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e9e-125">Response</span></span>

<span data-ttu-id="17e9e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17e9e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17e9e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17e9e-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="17e9e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17e9e-129">Request</span></span>

<span data-ttu-id="17e9e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="17e9e-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17e9e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="17e9e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17e9e-132">C#</span><span class="sxs-lookup"><span data-stu-id="17e9e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17e9e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17e9e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17e9e-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="17e9e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17e9e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="17e9e-135">Response</span></span>

<span data-ttu-id="17e9e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="17e9e-136">The following is an example of the response.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
