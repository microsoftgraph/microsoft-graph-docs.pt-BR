---
title: 'teamsAppInstallation: atualização'
description: Atualizar uma instalação de aplicativo em uma equipe
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3e75186223ebed0cf04c39c098ac970a9d9e2869
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607313"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="6458f-103">teamsAppInstallation: atualização</span><span class="sxs-lookup"><span data-stu-id="6458f-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="6458f-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6458f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6458f-105">Atualize uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6458f-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="6458f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6458f-106">Permissions</span></span>

<span data-ttu-id="6458f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6458f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6458f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6458f-109">Permission type</span></span>      | <span data-ttu-id="6458f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6458f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6458f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6458f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6458f-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6458f-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="6458f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6458f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6458f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6458f-114">Not supported.</span></span>    |
|<span data-ttu-id="6458f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6458f-115">Application</span></span> | <span data-ttu-id="6458f-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6458f-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6458f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6458f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="6458f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6458f-118">Request headers</span></span>

| <span data-ttu-id="6458f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6458f-119">Header</span></span>       | <span data-ttu-id="6458f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6458f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6458f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6458f-121">Authorization</span></span>  | <span data-ttu-id="6458f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6458f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6458f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6458f-124">Request body</span></span>

<span data-ttu-id="6458f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6458f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6458f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6458f-126">Response</span></span>

<span data-ttu-id="6458f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6458f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6458f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6458f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6458f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6458f-130">Request</span></span>

<span data-ttu-id="6458f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6458f-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp_in_team"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/db5e04be-daa2-4a35-beb1-5e73cc381599/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=/upgrade
```


### <a name="response"></a><span data-ttu-id="6458f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6458f-132">Response</span></span>

<span data-ttu-id="6458f-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6458f-133">The following is an example of the response.</span></span> 

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


