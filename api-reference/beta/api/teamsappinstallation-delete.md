---
title: Remover aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 574872a4b942aca4429ef856b10c41f4e4661f5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452544"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="1145e-103">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="1145e-103">Remove app from team</span></span>

<span data-ttu-id="1145e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1145e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1145e-105">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="1145e-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1145e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1145e-106">Permissions</span></span>

<span data-ttu-id="1145e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1145e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1145e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1145e-109">Permission type</span></span>      | <span data-ttu-id="1145e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1145e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1145e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1145e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1145e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1145e-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1145e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1145e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1145e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1145e-114">Not supported.</span></span>    |
|<span data-ttu-id="1145e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1145e-115">Application</span></span> | <span data-ttu-id="1145e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1145e-116">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1145e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1145e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1145e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1145e-118">Request headers</span></span>

| <span data-ttu-id="1145e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1145e-119">Header</span></span>       | <span data-ttu-id="1145e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1145e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1145e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1145e-121">Authorization</span></span>  | <span data-ttu-id="1145e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1145e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1145e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1145e-124">Request body</span></span>

<span data-ttu-id="1145e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1145e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1145e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1145e-126">Response</span></span>

<span data-ttu-id="1145e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1145e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1145e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1145e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1145e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1145e-130">Request</span></span>

<span data-ttu-id="1145e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1145e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1145e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1145e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="1145e-133">C#</span><span class="sxs-lookup"><span data-stu-id="1145e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1145e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1145e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1145e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1145e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1145e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1145e-136">Response</span></span>

<span data-ttu-id="1145e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1145e-137">The following is an example of the response.</span></span>

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
