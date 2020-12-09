---
title: Adicionar aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 056543a8b1753fb9a0b4bb6e8cdfe28428ae2e01
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607287"
---
# <a name="add-app-to-team"></a><span data-ttu-id="f725f-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="f725f-103">Add app to team</span></span>

<span data-ttu-id="f725f-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f725f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f725f-105">Instalar um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="f725f-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f725f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f725f-106">Permissions</span></span>

<span data-ttu-id="f725f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f725f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f725f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f725f-109">Permission type</span></span>      | <span data-ttu-id="f725f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f725f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f725f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f725f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f725f-112">TeamsAppInstallation. ReadWriteForTeam, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f725f-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f725f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f725f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f725f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f725f-114">Not supported.</span></span>    |
|<span data-ttu-id="f725f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f725f-115">Application</span></span> | <span data-ttu-id="f725f-116">TeamsAppInstallation. ReadWriteForTeam. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f725f-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f725f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f725f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="f725f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f725f-118">Request headers</span></span>

| <span data-ttu-id="f725f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f725f-119">Header</span></span>       | <span data-ttu-id="f725f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f725f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f725f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f725f-121">Authorization</span></span>  | <span data-ttu-id="f725f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f725f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f725f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f725f-124">Request body</span></span>

| <span data-ttu-id="f725f-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f725f-125">Property</span></span>   | <span data-ttu-id="f725f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f725f-126">Type</span></span> |<span data-ttu-id="f725f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f725f-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f725f-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f725f-128">teamsApp</span></span>|<span data-ttu-id="f725f-129">String</span><span class="sxs-lookup"><span data-stu-id="f725f-129">String</span></span>|<span data-ttu-id="f725f-130">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="f725f-130">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="f725f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f725f-131">Response</span></span>

<span data-ttu-id="f725f-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f725f-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f725f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f725f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f725f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f725f-135">Request</span></span>

<span data-ttu-id="f725f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f725f-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_app_in_team"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="f725f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f725f-137">Response</span></span>

<span data-ttu-id="f725f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f725f-138">The following is an example of the response.</span></span>

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


