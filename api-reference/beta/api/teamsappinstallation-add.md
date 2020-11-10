---
title: Adicionar aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f08581047327e1f9d49a46cd68996e6efed9f043
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981766"
---
# <a name="add-app-to-team"></a><span data-ttu-id="87971-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="87971-103">Add app to team</span></span>

<span data-ttu-id="87971-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87971-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87971-105">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="87971-105">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87971-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87971-106">Permissions</span></span>

<span data-ttu-id="87971-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87971-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87971-109">Permission type</span></span>      | <span data-ttu-id="87971-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87971-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87971-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87971-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87971-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="87971-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="87971-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87971-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87971-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87971-114">Not supported.</span></span>    |
|<span data-ttu-id="87971-115">Application</span><span class="sxs-lookup"><span data-stu-id="87971-115">Application</span></span> | <span data-ttu-id="87971-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="87971-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87971-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87971-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="87971-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87971-118">Request headers</span></span>

| <span data-ttu-id="87971-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87971-119">Header</span></span>       | <span data-ttu-id="87971-120">Valor</span><span class="sxs-lookup"><span data-stu-id="87971-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87971-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="87971-121">Authorization</span></span>  | <span data-ttu-id="87971-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87971-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87971-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87971-124">Request body</span></span>

| <span data-ttu-id="87971-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87971-125">Property</span></span>   | <span data-ttu-id="87971-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="87971-126">Type</span></span> |<span data-ttu-id="87971-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="87971-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87971-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="87971-128">teamsApp</span></span>|<span data-ttu-id="87971-129">String</span><span class="sxs-lookup"><span data-stu-id="87971-129">String</span></span>|<span data-ttu-id="87971-130">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="87971-130">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="87971-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="87971-131">Response</span></span>

<span data-ttu-id="87971-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87971-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87971-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87971-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="87971-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87971-135">Request</span></span>

<span data-ttu-id="87971-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87971-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87971-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="87971-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="87971-138">C#</span><span class="sxs-lookup"><span data-stu-id="87971-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87971-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87971-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87971-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87971-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87971-141">Java</span><span class="sxs-lookup"><span data-stu-id="87971-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87971-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="87971-142">Response</span></span>

<span data-ttu-id="87971-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87971-143">The following is an example of the response.</span></span>

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


