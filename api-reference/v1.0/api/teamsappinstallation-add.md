---
title: Adicionar aplicativo à equipe
description: Instalar um aplicativo para a equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fc5f92212d9fbeb6b061f952ff31c76fcf1f2ce8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375496"
---
# <a name="add-app-to-team"></a><span data-ttu-id="0371c-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="0371c-103">Add app to team</span></span>

<span data-ttu-id="0371c-104">Instalar um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="0371c-104">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0371c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0371c-105">Permissions</span></span>

<span data-ttu-id="0371c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0371c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0371c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0371c-108">Permission type</span></span>      | <span data-ttu-id="0371c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0371c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0371c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0371c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0371c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0371c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0371c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0371c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0371c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0371c-113">Not supported.</span></span>    |
|<span data-ttu-id="0371c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0371c-114">Application</span></span> | <span data-ttu-id="0371c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0371c-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0371c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0371c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="0371c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0371c-117">Request headers</span></span>

| <span data-ttu-id="0371c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0371c-118">Header</span></span>       | <span data-ttu-id="0371c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="0371c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0371c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0371c-120">Authorization</span></span>  | <span data-ttu-id="0371c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0371c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0371c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0371c-123">Request body</span></span>

| <span data-ttu-id="0371c-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0371c-124">Property</span></span>   | <span data-ttu-id="0371c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0371c-125">Type</span></span> |<span data-ttu-id="0371c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0371c-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0371c-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0371c-127">teamsApp</span></span>| [<span data-ttu-id="0371c-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0371c-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="0371c-129">O aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="0371c-129">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="0371c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0371c-130">Response</span></span>

<span data-ttu-id="0371c-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0371c-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0371c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0371c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0371c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0371c-134">Request</span></span>

<span data-ttu-id="0371c-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0371c-135">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0371c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0371c-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0371c-137">C#</span><span class="sxs-lookup"><span data-stu-id="0371c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0371c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0371c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0371c-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0371c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0371c-140">Java</span><span class="sxs-lookup"><span data-stu-id="0371c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0371c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0371c-141">Response</span></span>

<span data-ttu-id="0371c-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0371c-142">The following is an example of the response.</span></span>

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
