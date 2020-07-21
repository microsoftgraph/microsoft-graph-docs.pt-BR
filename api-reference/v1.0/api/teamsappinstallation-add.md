---
title: Adicionar aplicativo à equipe
description: Instalar um aplicativo para a equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ea69b69718afefdaf54b80ac985598c9173081d8
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/21/2020
ms.locfileid: "45197076"
---
# <a name="add-app-to-team"></a><span data-ttu-id="c5603-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="c5603-103">Add app to team</span></span>

<span data-ttu-id="c5603-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5603-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5603-105">Instalar um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="c5603-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5603-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5603-106">Permissions</span></span>

<span data-ttu-id="c5603-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5603-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5603-109">Permission type</span></span>      | <span data-ttu-id="c5603-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5603-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5603-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5603-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5603-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c5603-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="c5603-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5603-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5603-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5603-114">Not supported.</span></span>    |
|<span data-ttu-id="c5603-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5603-115">Application</span></span> | <span data-ttu-id="c5603-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c5603-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5603-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5603-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="c5603-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5603-118">Request headers</span></span>

| <span data-ttu-id="c5603-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5603-119">Header</span></span>       | <span data-ttu-id="c5603-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c5603-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5603-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5603-121">Authorization</span></span>  | <span data-ttu-id="c5603-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5603-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5603-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5603-124">Request body</span></span>

| <span data-ttu-id="c5603-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5603-125">Property</span></span>   | <span data-ttu-id="c5603-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5603-126">Type</span></span> |<span data-ttu-id="c5603-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5603-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5603-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c5603-128">teamsApp</span></span>| [<span data-ttu-id="c5603-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c5603-129">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="c5603-130">O aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="c5603-130">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="c5603-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5603-131">Response</span></span>

<span data-ttu-id="c5603-p103">Se bem-sucedido, este método retorna um código de resposta `201 Created`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5603-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5603-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5603-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5603-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5603-135">Request</span></span>

<span data-ttu-id="c5603-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5603-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c5603-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5603-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c5603-138">C#</span><span class="sxs-lookup"><span data-stu-id="c5603-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5603-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5603-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5603-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5603-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5603-141">Java</span><span class="sxs-lookup"><span data-stu-id="c5603-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5603-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5603-142">Response</span></span>

<span data-ttu-id="c5603-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5603-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
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
