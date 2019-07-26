---
title: Desinstalar o aplicativo para o usuário
description: Desinstala um aplicativo do escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 42030378f3d66c11d1d9f8d8856739c54508c302
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908527"
---
# <a name="uninstall-app-for-user"></a><span data-ttu-id="12526-103">Desinstalar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="12526-103">Uninstall app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12526-104">Desinstala um [aplicativo](../resources/teamsappinstallation.md) do escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="12526-104">Uninstall an [app](../resources/teamsappinstallation.md) from the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="12526-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="12526-105">Permissions</span></span>

<span data-ttu-id="12526-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12526-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12526-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12526-108">Permission type</span></span>      | <span data-ttu-id="12526-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12526-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12526-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12526-110">Delegated (work or school account)</span></span> |<span data-ttu-id="12526-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12526-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="12526-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12526-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12526-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12526-113">Not supported.</span></span>    |
|<span data-ttu-id="12526-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12526-114">Application</span></span> | <span data-ttu-id="12526-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12526-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="12526-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12526-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="12526-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12526-117">Request headers</span></span>

| <span data-ttu-id="12526-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12526-118">Header</span></span>       | <span data-ttu-id="12526-119">Valor</span><span class="sxs-lookup"><span data-stu-id="12526-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12526-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="12526-120">Authorization</span></span>  | <span data-ttu-id="12526-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12526-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12526-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12526-123">Request body</span></span>

<span data-ttu-id="12526-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12526-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12526-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="12526-125">Response</span></span>

<span data-ttu-id="12526-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12526-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12526-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12526-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="12526-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12526-129">Request</span></span>

<span data-ttu-id="12526-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="12526-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```

### <a name="response"></a><span data-ttu-id="12526-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="12526-131">Response</span></span>

<span data-ttu-id="12526-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="12526-132">The following is an example of the response.</span></span>

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
