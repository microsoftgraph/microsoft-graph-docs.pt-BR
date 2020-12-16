---
title: Remover aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6d51730971ad26bb7f5de5479d4c95aaa874fd00
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690640"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="a4f3d-103">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="a4f3d-103">Remove app from team</span></span>

<span data-ttu-id="a4f3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4f3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4f3d-105">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="a4f3d-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4f3d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a4f3d-106">Permissions</span></span>

<span data-ttu-id="a4f3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4f3d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4f3d-109">Permission type</span></span>      | <span data-ttu-id="a4f3d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4f3d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4f3d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4f3d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4f3d-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a4f3d-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a4f3d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4f3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4f3d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4f3d-114">Not supported.</span></span>    |
|<span data-ttu-id="a4f3d-115">Application</span><span class="sxs-lookup"><span data-stu-id="a4f3d-115">Application</span></span> | <span data-ttu-id="a4f3d-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a4f3d-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4f3d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4f3d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="a4f3d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4f3d-118">Request headers</span></span>

| <span data-ttu-id="a4f3d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4f3d-119">Header</span></span>       | <span data-ttu-id="a4f3d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a4f3d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4f3d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4f3d-121">Authorization</span></span>  | <span data-ttu-id="a4f3d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4f3d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4f3d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4f3d-124">Request body</span></span>

<span data-ttu-id="a4f3d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4f3d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4f3d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4f3d-126">Response</span></span>

<span data-ttu-id="a4f3d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4f3d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4f3d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4f3d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4f3d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4f3d-130">Request</span></span>

<span data-ttu-id="a4f3d-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4f3d-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a4f3d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4f3d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp_in_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```
# <a name="c"></a>[<span data-ttu-id="a4f3d-133">C#</span><span class="sxs-lookup"><span data-stu-id="a4f3d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4f3d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4f3d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4f3d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4f3d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4f3d-136">Java</span><span class="sxs-lookup"><span data-stu-id="a4f3d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4f3d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4f3d-137">Response</span></span>

<span data-ttu-id="a4f3d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a4f3d-138">The following is an example of the response.</span></span>

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


