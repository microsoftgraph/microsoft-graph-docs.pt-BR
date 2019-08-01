---
title: Adicionar aplicativo à equipe
description: Instalar um aplicativo para a equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: df830e1be8eac1e098e687b640b987c71f473ed1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027318"
---
# <a name="add-app-to-team"></a><span data-ttu-id="3cd5e-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="3cd5e-103">Add app to team</span></span>

<span data-ttu-id="3cd5e-104">Instalar um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="3cd5e-104">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3cd5e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cd5e-105">Permissions</span></span>

<span data-ttu-id="3cd5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cd5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd5e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cd5e-108">Permission type</span></span>      | <span data-ttu-id="3cd5e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cd5e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cd5e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cd5e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3cd5e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd5e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3cd5e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cd5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cd5e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd5e-113">Not supported.</span></span>    |
|<span data-ttu-id="3cd5e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cd5e-114">Application</span></span> | <span data-ttu-id="3cd5e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd5e-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cd5e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd5e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="3cd5e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd5e-117">Request headers</span></span>

| <span data-ttu-id="3cd5e-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cd5e-118">Header</span></span>       | <span data-ttu-id="3cd5e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="3cd5e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3cd5e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cd5e-120">Authorization</span></span>  | <span data-ttu-id="3cd5e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cd5e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cd5e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd5e-123">Request body</span></span>

| <span data-ttu-id="3cd5e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cd5e-124">Property</span></span>   | <span data-ttu-id="3cd5e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cd5e-125">Type</span></span> |<span data-ttu-id="3cd5e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd5e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cd5e-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3cd5e-127">teamsApp</span></span>| [<span data-ttu-id="3cd5e-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3cd5e-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="3cd5e-129">O aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="3cd5e-129">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="3cd5e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd5e-130">Response</span></span>

<span data-ttu-id="3cd5e-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd5e-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cd5e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cd5e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cd5e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd5e-134">Request</span></span>

<span data-ttu-id="3cd5e-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cd5e-135">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3cd5e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd5e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3cd5e-137">C#</span><span class="sxs-lookup"><span data-stu-id="3cd5e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cd5e-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cd5e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3cd5e-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3cd5e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3cd5e-140">Java</span><span class="sxs-lookup"><span data-stu-id="3cd5e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3cd5e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd5e-141">Response</span></span>

<span data-ttu-id="3cd5e-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3cd5e-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
