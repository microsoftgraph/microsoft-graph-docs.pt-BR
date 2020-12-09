---
title: Adicionar aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8fde83a82e1c46b8b37cfedea2a202b8d339ea2d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607506"
---
# <a name="add-app-to-team"></a><span data-ttu-id="13dc0-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="13dc0-103">Add app to team</span></span>

<span data-ttu-id="13dc0-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="13dc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13dc0-105">Instalar um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="13dc0-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13dc0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="13dc0-106">Permissions</span></span>

<span data-ttu-id="13dc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13dc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13dc0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13dc0-109">Permission type</span></span>      | <span data-ttu-id="13dc0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13dc0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13dc0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13dc0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="13dc0-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="13dc0-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="13dc0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13dc0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13dc0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13dc0-114">Not supported.</span></span>    |
|<span data-ttu-id="13dc0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13dc0-115">Application</span></span> | <span data-ttu-id="13dc0-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="13dc0-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13dc0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13dc0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="13dc0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13dc0-118">Request headers</span></span>

| <span data-ttu-id="13dc0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13dc0-119">Header</span></span>       | <span data-ttu-id="13dc0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="13dc0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13dc0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="13dc0-121">Authorization</span></span>  | <span data-ttu-id="13dc0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13dc0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13dc0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13dc0-124">Request body</span></span>

| <span data-ttu-id="13dc0-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13dc0-125">Property</span></span>   | <span data-ttu-id="13dc0-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="13dc0-126">Type</span></span> |<span data-ttu-id="13dc0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="13dc0-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13dc0-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="13dc0-128">teamsApp</span></span>|<span data-ttu-id="13dc0-129">String</span><span class="sxs-lookup"><span data-stu-id="13dc0-129">String</span></span>|<span data-ttu-id="13dc0-130">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="13dc0-130">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="13dc0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="13dc0-131">Response</span></span>

<span data-ttu-id="13dc0-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13dc0-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13dc0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13dc0-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="13dc0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13dc0-135">Request</span></span>

<span data-ttu-id="13dc0-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="13dc0-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_app_in_team"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="13dc0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="13dc0-137">Response</span></span>

<span data-ttu-id="13dc0-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13dc0-138">The following is an example of the response.</span></span>

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


