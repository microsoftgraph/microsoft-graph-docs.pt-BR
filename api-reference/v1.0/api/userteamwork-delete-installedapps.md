---
title: Desinstalar o aplicativo para o usuário
description: Desinstale um aplicativo do escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c27b1fde186141d7eadc606a3fbd19dd16fae92c
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607193"
---
# <a name="uninstall-app-for-user"></a><span data-ttu-id="a9483-103">Desinstalar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="a9483-103">Uninstall app for user</span></span>

<span data-ttu-id="a9483-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a9483-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9483-105">Desinstala um [aplicativo](../resources/teamsappinstallation.md) do escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="a9483-105">Uninstall an [app](../resources/teamsappinstallation.md) from the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9483-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a9483-106">Permissions</span></span>

<span data-ttu-id="a9483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9483-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9483-109">Permission type</span></span>      | <span data-ttu-id="a9483-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9483-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9483-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9483-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9483-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="a9483-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="a9483-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9483-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9483-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9483-114">Not supported.</span></span>    |
|<span data-ttu-id="a9483-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9483-115">Application</span></span> | <span data-ttu-id="a9483-116">TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All</span><span class="sxs-lookup"><span data-stu-id="a9483-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9483-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9483-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{user-id}/teamwork/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="a9483-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9483-118">Request headers</span></span>

| <span data-ttu-id="a9483-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9483-119">Header</span></span>       | <span data-ttu-id="a9483-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a9483-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9483-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9483-121">Authorization</span></span>  | <span data-ttu-id="a9483-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9483-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9483-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9483-124">Request body</span></span>

<span data-ttu-id="a9483-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9483-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9483-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9483-126">Response</span></span>

<span data-ttu-id="a9483-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9483-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9483-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9483-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9483-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9483-130">Request</span></span>

<span data-ttu-id="a9483-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9483-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk
```

### <a name="response"></a><span data-ttu-id="a9483-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9483-132">Response</span></span>

<span data-ttu-id="a9483-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9483-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User delete teamsAppInstallations,
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
