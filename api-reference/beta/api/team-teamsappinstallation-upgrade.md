---
title: 'teamsAppInstallation: upgrade'
description: Atualizar uma instalação de aplicativo em uma equipe
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1be01afcd09e7870af75b4c3a5b4eb9a481bc78c
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691043"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="99552-103">teamsAppInstallation: upgrade</span><span class="sxs-lookup"><span data-stu-id="99552-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="99552-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99552-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99552-105">Atualize uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="99552-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="99552-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="99552-106">Permissions</span></span>

<span data-ttu-id="99552-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99552-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99552-109">Permission type</span></span>      | <span data-ttu-id="99552-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99552-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99552-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99552-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99552-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="99552-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="99552-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99552-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99552-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99552-114">Not supported.</span></span>    |
|<span data-ttu-id="99552-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99552-115">Application</span></span> | <span data-ttu-id="99552-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="99552-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99552-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99552-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="99552-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99552-118">Request headers</span></span>

| <span data-ttu-id="99552-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99552-119">Header</span></span>       | <span data-ttu-id="99552-120">Valor</span><span class="sxs-lookup"><span data-stu-id="99552-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99552-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="99552-121">Authorization</span></span>  | <span data-ttu-id="99552-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99552-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99552-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99552-124">Request body</span></span>

<span data-ttu-id="99552-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99552-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99552-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="99552-126">Response</span></span>

<span data-ttu-id="99552-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99552-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99552-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99552-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="99552-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99552-130">Request</span></span>

<span data-ttu-id="99552-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="99552-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="99552-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="99552-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp_in_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/db5e04be-daa2-4a35-beb1-5e73cc381599/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=/upgrade
```
# <a name="c"></a>[<span data-ttu-id="99552-133">C#</span><span class="sxs-lookup"><span data-stu-id="99552-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99552-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99552-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99552-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99552-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99552-136">Java</span><span class="sxs-lookup"><span data-stu-id="99552-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="99552-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="99552-137">Response</span></span>

<span data-ttu-id="99552-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="99552-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp_in_team",
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
  "description": "Upgrade app in team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


