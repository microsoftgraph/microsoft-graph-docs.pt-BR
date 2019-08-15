---
title: Remover aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8e86ef713cee1f638f626a3475afc341b9aa9cb5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421341"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="0795b-103">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="0795b-103">Remove app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0795b-104">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="0795b-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0795b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0795b-105">Permissions</span></span>

<span data-ttu-id="0795b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0795b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0795b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0795b-108">Permission type</span></span>      | <span data-ttu-id="0795b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0795b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0795b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0795b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0795b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0795b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0795b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0795b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0795b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0795b-113">Not supported.</span></span>    |
|<span data-ttu-id="0795b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0795b-114">Application</span></span> | <span data-ttu-id="0795b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0795b-115">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0795b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0795b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0795b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0795b-117">Request headers</span></span>

| <span data-ttu-id="0795b-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0795b-118">Header</span></span>       | <span data-ttu-id="0795b-119">Valor</span><span class="sxs-lookup"><span data-stu-id="0795b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0795b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0795b-120">Authorization</span></span>  | <span data-ttu-id="0795b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0795b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0795b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0795b-123">Request body</span></span>

<span data-ttu-id="0795b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0795b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0795b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0795b-125">Response</span></span>

<span data-ttu-id="0795b-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0795b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0795b-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0795b-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="0795b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0795b-129">Request</span></span>

<span data-ttu-id="0795b-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0795b-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0795b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0795b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0795b-132">C#</span><span class="sxs-lookup"><span data-stu-id="0795b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0795b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0795b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0795b-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0795b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0795b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0795b-135">Response</span></span>

<span data-ttu-id="0795b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0795b-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp",
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
