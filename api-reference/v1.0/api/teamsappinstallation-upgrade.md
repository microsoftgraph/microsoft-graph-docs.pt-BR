---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4ab3a2bdce05e6cbe6b653109ef0e8faed9946e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509283"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="7cf5d-103">Atualizar um aplicativo em uma equipe</span><span class="sxs-lookup"><span data-stu-id="7cf5d-103">Upgrade an app in a team</span></span>

<span data-ttu-id="7cf5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cf5d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7cf5d-105">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7cf5d-105">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cf5d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cf5d-106">Permissions</span></span>

<span data-ttu-id="7cf5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cf5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cf5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cf5d-109">Permission type</span></span>      | <span data-ttu-id="7cf5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cf5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cf5d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cf5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7cf5d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf5d-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7cf5d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cf5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cf5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cf5d-114">Not supported.</span></span>    |
|<span data-ttu-id="7cf5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cf5d-115">Application</span></span> | <span data-ttu-id="7cf5d-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf5d-116">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="7cf5d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf5d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="7cf5d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf5d-118">Request headers</span></span>

| <span data-ttu-id="7cf5d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cf5d-119">Header</span></span>       | <span data-ttu-id="7cf5d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7cf5d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7cf5d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cf5d-121">Authorization</span></span>  | <span data-ttu-id="7cf5d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cf5d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7cf5d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf5d-124">Request body</span></span>

<span data-ttu-id="7cf5d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7cf5d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cf5d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf5d-126">Response</span></span>

<span data-ttu-id="7cf5d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cf5d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cf5d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cf5d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cf5d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf5d-130">Request</span></span>

<span data-ttu-id="7cf5d-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cf5d-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7cf5d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf5d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="7cf5d-133">C#</span><span class="sxs-lookup"><span data-stu-id="7cf5d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cf5d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cf5d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cf5d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cf5d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cf5d-136">Java</span><span class="sxs-lookup"><span data-stu-id="7cf5d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7cf5d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf5d-137">Response</span></span>

<span data-ttu-id="7cf5d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7cf5d-138">The following is an example of the response.</span></span> 

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
