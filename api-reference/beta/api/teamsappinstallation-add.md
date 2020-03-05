---
title: Adicionar aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f50faf97aed8031525b27d90acd31639a3d6025
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452523"
---
# <a name="add-app-to-team"></a><span data-ttu-id="ab3e1-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="ab3e1-103">Add app to team</span></span>

<span data-ttu-id="ab3e1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab3e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab3e1-105">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="ab3e1-105">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab3e1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab3e1-106">Permissions</span></span>

<span data-ttu-id="ab3e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab3e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab3e1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab3e1-109">Permission type</span></span>      | <span data-ttu-id="ab3e1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab3e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab3e1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab3e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab3e1-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3e1-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab3e1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab3e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab3e1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab3e1-114">Not supported.</span></span>    |
|<span data-ttu-id="ab3e1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab3e1-115">Application</span></span> | <span data-ttu-id="ab3e1-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3e1-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab3e1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab3e1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="ab3e1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab3e1-118">Request headers</span></span>

| <span data-ttu-id="ab3e1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab3e1-119">Header</span></span>       | <span data-ttu-id="ab3e1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ab3e1-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab3e1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab3e1-121">Authorization</span></span>  | <span data-ttu-id="ab3e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab3e1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab3e1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab3e1-124">Request body</span></span>

| <span data-ttu-id="ab3e1-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab3e1-125">Property</span></span>   | <span data-ttu-id="ab3e1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab3e1-126">Type</span></span> |<span data-ttu-id="ab3e1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab3e1-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab3e1-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ab3e1-128">teamsApp</span></span>|<span data-ttu-id="ab3e1-129">String</span><span class="sxs-lookup"><span data-stu-id="ab3e1-129">String</span></span>|<span data-ttu-id="ab3e1-130">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ab3e1-130">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="ab3e1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab3e1-131">Response</span></span>

<span data-ttu-id="ab3e1-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab3e1-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab3e1-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab3e1-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab3e1-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab3e1-135">Request</span></span>

<span data-ttu-id="ab3e1-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab3e1-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab3e1-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab3e1-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_teamsApp"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="ab3e1-138">C#</span><span class="sxs-lookup"><span data-stu-id="ab3e1-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab3e1-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab3e1-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab3e1-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab3e1-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab3e1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab3e1-141">Response</span></span>

<span data-ttu-id="ab3e1-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab3e1-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add teamsApp",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
