---
title: Remover aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e7a17cbd71635f820f0d2580efdb8cf2f74c03bb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362826"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="98a74-103">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="98a74-103">Remove app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98a74-104">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="98a74-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="98a74-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="98a74-105">Permissions</span></span>

<span data-ttu-id="98a74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98a74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98a74-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98a74-108">Permission type</span></span>      | <span data-ttu-id="98a74-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98a74-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98a74-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98a74-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98a74-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98a74-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="98a74-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98a74-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98a74-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98a74-113">Not supported.</span></span>    |
|<span data-ttu-id="98a74-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98a74-114">Application</span></span> | <span data-ttu-id="98a74-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98a74-115">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="98a74-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98a74-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="98a74-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98a74-117">Request headers</span></span>

| <span data-ttu-id="98a74-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98a74-118">Header</span></span>       | <span data-ttu-id="98a74-119">Valor</span><span class="sxs-lookup"><span data-stu-id="98a74-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98a74-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="98a74-120">Authorization</span></span>  | <span data-ttu-id="98a74-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98a74-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98a74-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98a74-123">Request body</span></span>

<span data-ttu-id="98a74-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98a74-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98a74-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="98a74-125">Response</span></span>

<span data-ttu-id="98a74-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98a74-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98a74-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98a74-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="98a74-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98a74-129">Request</span></span>

<span data-ttu-id="98a74-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="98a74-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98a74-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="98a74-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98a74-132">C#</span><span class="sxs-lookup"><span data-stu-id="98a74-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98a74-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98a74-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98a74-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="98a74-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="98a74-135">Java</span><span class="sxs-lookup"><span data-stu-id="98a74-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98a74-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="98a74-136">Response</span></span>

<span data-ttu-id="98a74-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="98a74-137">The following is an example of the response.</span></span>

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
