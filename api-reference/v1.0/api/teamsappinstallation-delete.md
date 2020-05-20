---
title: Remover aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 49202697c16236df9c06b7f2f36b49c8763b54a8
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290425"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="45545-103">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="45545-103">Remove app from team</span></span>

<span data-ttu-id="45545-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45545-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45545-105">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="45545-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45545-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45545-106">Permissions</span></span>

<span data-ttu-id="45545-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45545-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45545-109">Permission type</span></span>      | <span data-ttu-id="45545-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45545-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45545-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45545-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45545-112">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45545-112">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="45545-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45545-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45545-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45545-114">Not supported.</span></span>    |
|<span data-ttu-id="45545-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45545-115">Application</span></span> | <span data-ttu-id="45545-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45545-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45545-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45545-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="45545-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45545-118">Request headers</span></span>

| <span data-ttu-id="45545-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45545-119">Header</span></span>       | <span data-ttu-id="45545-120">Valor</span><span class="sxs-lookup"><span data-stu-id="45545-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="45545-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="45545-121">Authorization</span></span>  | <span data-ttu-id="45545-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45545-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45545-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45545-124">Request body</span></span>

<span data-ttu-id="45545-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45545-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45545-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="45545-126">Response</span></span>

<span data-ttu-id="45545-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45545-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45545-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45545-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="45545-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45545-130">Request</span></span>

<span data-ttu-id="45545-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45545-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45545-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="45545-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->

```http
DELETE /teams/{id}/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="45545-133">C#</span><span class="sxs-lookup"><span data-stu-id="45545-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45545-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45545-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45545-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45545-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45545-136">Java</span><span class="sxs-lookup"><span data-stu-id="45545-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45545-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="45545-137">Response</span></span>

<span data-ttu-id="45545-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45545-138">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
