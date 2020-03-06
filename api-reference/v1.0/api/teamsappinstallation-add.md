---
title: Adicionar aplicativo à equipe
description: Instalar um aplicativo para a equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 85b0a94c3892bd31ff89d286697a7193a62cd771
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509304"
---
# <a name="add-app-to-team"></a><span data-ttu-id="ad12d-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="ad12d-103">Add app to team</span></span>

<span data-ttu-id="ad12d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad12d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad12d-105">Instalar um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="ad12d-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad12d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad12d-106">Permissions</span></span>

<span data-ttu-id="ad12d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad12d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad12d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad12d-109">Permission type</span></span>      | <span data-ttu-id="ad12d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad12d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad12d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad12d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad12d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad12d-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad12d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad12d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad12d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad12d-114">Not supported.</span></span>    |
|<span data-ttu-id="ad12d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad12d-115">Application</span></span> | <span data-ttu-id="ad12d-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad12d-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad12d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad12d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="ad12d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad12d-118">Request headers</span></span>

| <span data-ttu-id="ad12d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad12d-119">Header</span></span>       | <span data-ttu-id="ad12d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ad12d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad12d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad12d-121">Authorization</span></span>  | <span data-ttu-id="ad12d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad12d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad12d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad12d-124">Request body</span></span>

| <span data-ttu-id="ad12d-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad12d-125">Property</span></span>   | <span data-ttu-id="ad12d-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad12d-126">Type</span></span> |<span data-ttu-id="ad12d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad12d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad12d-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ad12d-128">teamsApp</span></span>| [<span data-ttu-id="ad12d-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ad12d-129">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="ad12d-130">O aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="ad12d-130">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="ad12d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad12d-131">Response</span></span>

<span data-ttu-id="ad12d-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad12d-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad12d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad12d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad12d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad12d-135">Request</span></span>

<span data-ttu-id="ad12d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad12d-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad12d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad12d-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ad12d-138">C#</span><span class="sxs-lookup"><span data-stu-id="ad12d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad12d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad12d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad12d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad12d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad12d-141">Java</span><span class="sxs-lookup"><span data-stu-id="ad12d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad12d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad12d-142">Response</span></span>

<span data-ttu-id="ad12d-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ad12d-143">The following is an example of the response.</span></span>

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
