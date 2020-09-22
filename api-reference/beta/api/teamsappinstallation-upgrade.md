---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 967eb8092e5cf7e971ecc690dded4dbae3578f52
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999066"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="3ad9f-103">Atualizar um aplicativo em uma equipe</span><span class="sxs-lookup"><span data-stu-id="3ad9f-103">Upgrade an app in a team</span></span>

<span data-ttu-id="3ad9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ad9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ad9f-105">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ad9f-105">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ad9f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ad9f-106">Permissions</span></span>

<span data-ttu-id="3ad9f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ad9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ad9f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ad9f-109">Permission type</span></span>      | <span data-ttu-id="3ad9f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ad9f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ad9f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ad9f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ad9f-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3ad9f-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3ad9f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ad9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ad9f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ad9f-114">Not supported.</span></span>    |
|<span data-ttu-id="3ad9f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ad9f-115">Application</span></span> | <span data-ttu-id="3ad9f-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3ad9f-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ad9f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ad9f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="3ad9f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ad9f-118">Request headers</span></span>

| <span data-ttu-id="3ad9f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ad9f-119">Header</span></span>       | <span data-ttu-id="3ad9f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3ad9f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ad9f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ad9f-121">Authorization</span></span>  | <span data-ttu-id="3ad9f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ad9f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ad9f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ad9f-124">Request body</span></span>

<span data-ttu-id="3ad9f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ad9f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ad9f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ad9f-126">Response</span></span>

<span data-ttu-id="3ad9f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ad9f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ad9f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ad9f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ad9f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ad9f-130">Request</span></span>

<span data-ttu-id="3ad9f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ad9f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ad9f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ad9f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="3ad9f-133">C#</span><span class="sxs-lookup"><span data-stu-id="3ad9f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ad9f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ad9f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ad9f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ad9f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3ad9f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ad9f-136">Response</span></span>

<span data-ttu-id="3ad9f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ad9f-137">The following is an example of the response.</span></span> 

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


