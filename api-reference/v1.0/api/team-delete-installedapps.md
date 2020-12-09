---
title: Remover aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 159f355514cab6f1ffb230f26c95208e58e416b6
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607308"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="8e8a6-103">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="8e8a6-103">Remove app from team</span></span>

<span data-ttu-id="8e8a6-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8e8a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e8a6-105">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="8e8a6-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e8a6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8e8a6-106">Permissions</span></span>

<span data-ttu-id="8e8a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e8a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e8a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e8a6-109">Permission type</span></span>      | <span data-ttu-id="8e8a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e8a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e8a6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e8a6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8e8a6-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8e8a6-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="8e8a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e8a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e8a6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e8a6-114">Not supported.</span></span>    |
|<span data-ttu-id="8e8a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e8a6-115">Application</span></span> | <span data-ttu-id="8e8a6-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8e8a6-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e8a6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e8a6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="8e8a6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8a6-118">Request headers</span></span>

| <span data-ttu-id="8e8a6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e8a6-119">Header</span></span>       | <span data-ttu-id="8e8a6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8e8a6-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e8a6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e8a6-121">Authorization</span></span>  | <span data-ttu-id="8e8a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e8a6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e8a6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8a6-124">Request body</span></span>

<span data-ttu-id="8e8a6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e8a6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e8a6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8a6-126">Response</span></span>

<span data-ttu-id="8e8a6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e8a6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e8a6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e8a6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e8a6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e8a6-130">Request</span></span>

<span data-ttu-id="8e8a6-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e8a6-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp_in_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```

### <a name="response"></a><span data-ttu-id="8e8a6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e8a6-132">Response</span></span>

<span data-ttu-id="8e8a6-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e8a6-133">The following is an example of the response.</span></span>

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


