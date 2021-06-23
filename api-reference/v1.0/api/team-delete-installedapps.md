---
title: Remover aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: akjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 768c7e58ff55ff01b48462c3ff621a95f066a247
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059457"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="50d6f-103">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="50d6f-103">Remove app from team</span></span>

<span data-ttu-id="50d6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50d6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50d6f-105">Desinstala [um aplicativo](../resources/teamsappinstallation.md) da equipe [especificada.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="50d6f-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="50d6f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="50d6f-106">Permissions</span></span>

<span data-ttu-id="50d6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50d6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d6f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50d6f-109">Permission type</span></span>      | <span data-ttu-id="50d6f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50d6f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50d6f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50d6f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50d6f-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d6f-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="50d6f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50d6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50d6f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50d6f-114">Not supported.</span></span>    |
|<span data-ttu-id="50d6f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50d6f-115">Application</span></span> | <span data-ttu-id="50d6f-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d6f-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50d6f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50d6f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="50d6f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50d6f-118">Request headers</span></span>

| <span data-ttu-id="50d6f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50d6f-119">Header</span></span>       | <span data-ttu-id="50d6f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="50d6f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50d6f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50d6f-121">Authorization</span></span>  | <span data-ttu-id="50d6f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50d6f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50d6f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50d6f-124">Request body</span></span>

<span data-ttu-id="50d6f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50d6f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50d6f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="50d6f-126">Response</span></span>

<span data-ttu-id="50d6f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50d6f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d6f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50d6f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="50d6f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50d6f-130">Request</span></span>

<span data-ttu-id="50d6f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="50d6f-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50d6f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="50d6f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp_in_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```
# <a name="c"></a>[<span data-ttu-id="50d6f-133">C#</span><span class="sxs-lookup"><span data-stu-id="50d6f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50d6f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50d6f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50d6f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50d6f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50d6f-136">Java</span><span class="sxs-lookup"><span data-stu-id="50d6f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50d6f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="50d6f-137">Response</span></span>

<span data-ttu-id="50d6f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="50d6f-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp_in_team",
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
  "description": "Remove app from team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


