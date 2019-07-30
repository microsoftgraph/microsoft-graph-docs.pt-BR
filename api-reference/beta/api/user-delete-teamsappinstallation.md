---
title: Desinstalar o aplicativo para o usuário
description: Desinstala um aplicativo do escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 78a8114d83e031416e1efafeaa2ec092107d91ee
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931615"
---
# <a name="uninstall-app-for-user"></a><span data-ttu-id="eb13b-103">Desinstalar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="eb13b-103">Uninstall app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb13b-104">Desinstala um [aplicativo](../resources/teamsappinstallation.md) do escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="eb13b-104">Uninstall an [app](../resources/teamsappinstallation.md) from the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb13b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb13b-105">Permissions</span></span>

<span data-ttu-id="eb13b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb13b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb13b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb13b-108">Permission type</span></span>      | <span data-ttu-id="eb13b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb13b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb13b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb13b-110">Delegated (work or school account)</span></span> |<span data-ttu-id="eb13b-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb13b-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb13b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb13b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb13b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb13b-113">Not supported.</span></span>    |
|<span data-ttu-id="eb13b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb13b-114">Application</span></span> | <span data-ttu-id="eb13b-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb13b-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="eb13b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb13b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eb13b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb13b-117">Request headers</span></span>

| <span data-ttu-id="eb13b-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb13b-118">Header</span></span>       | <span data-ttu-id="eb13b-119">Valor</span><span class="sxs-lookup"><span data-stu-id="eb13b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb13b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb13b-120">Authorization</span></span>  | <span data-ttu-id="eb13b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb13b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb13b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb13b-123">Request body</span></span>

<span data-ttu-id="eb13b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb13b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb13b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb13b-125">Response</span></span>

<span data-ttu-id="eb13b-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb13b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb13b-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb13b-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb13b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb13b-129">Request</span></span>

<span data-ttu-id="eb13b-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb13b-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eb13b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb13b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb13b-132">C#</span><span class="sxs-lookup"><span data-stu-id="eb13b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb13b-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb13b-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb13b-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eb13b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eb13b-135">Java</span><span class="sxs-lookup"><span data-stu-id="eb13b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb13b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb13b-136">Response</span></span>

<span data-ttu-id="eb13b-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb13b-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User delete teamsAppInstallations,
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
