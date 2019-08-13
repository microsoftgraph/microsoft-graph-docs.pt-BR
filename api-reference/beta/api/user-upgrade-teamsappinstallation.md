---
title: 'teamsAppInstallation: atualização'
description: Atualizar uma instalação de aplicativo no escopo pessoal de um usuário
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e0de5b95f8da705b6209cdaa5350f71d629a48f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362045"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="4f67f-103">teamsAppInstallation: atualização</span><span class="sxs-lookup"><span data-stu-id="4f67f-103">teamsAppInstallation: upgrade</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f67f-104">Atualize uma [instalação de aplicativo](../resources/teamsappinstallation.md) no escopo pessoal do [usuário](../resources/user.md) especificado para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f67f-104">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f67f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f67f-105">Permissions</span></span>

<span data-ttu-id="4f67f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f67f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f67f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f67f-108">Permission type</span></span>      | <span data-ttu-id="4f67f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f67f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f67f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f67f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f67f-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f67f-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="4f67f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f67f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f67f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f67f-113">Not supported.</span></span>    |
|<span data-ttu-id="4f67f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f67f-114">Application</span></span> | <span data-ttu-id="4f67f-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f67f-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f67f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f67f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="4f67f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f67f-117">Request headers</span></span>

| <span data-ttu-id="4f67f-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f67f-118">Header</span></span>       | <span data-ttu-id="4f67f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="4f67f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f67f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f67f-120">Authorization</span></span>  | <span data-ttu-id="4f67f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f67f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f67f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f67f-123">Request body</span></span>

<span data-ttu-id="4f67f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f67f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f67f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f67f-125">Response</span></span>

<span data-ttu-id="4f67f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f67f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f67f-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f67f-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f67f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f67f-129">Request</span></span>

<span data-ttu-id="4f67f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f67f-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4f67f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f67f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f67f-132">C#</span><span class="sxs-lookup"><span data-stu-id="4f67f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f67f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f67f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f67f-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4f67f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f67f-135">Java</span><span class="sxs-lookup"><span data-stu-id="4f67f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f67f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f67f-136">Response</span></span>

<span data-ttu-id="4f67f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f67f-137">The following is an example of the response.</span></span>

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
