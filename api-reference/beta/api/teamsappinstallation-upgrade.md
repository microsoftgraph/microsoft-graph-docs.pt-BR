---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f40951eb3c33b638542a8e2210911adffb15a444
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908323"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="7af5c-103">Atualizar um aplicativo em uma equipe</span><span class="sxs-lookup"><span data-stu-id="7af5c-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7af5c-104">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7af5c-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="7af5c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7af5c-105">Permissions</span></span>

<span data-ttu-id="7af5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7af5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7af5c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7af5c-108">Permission type</span></span>      | <span data-ttu-id="7af5c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7af5c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7af5c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7af5c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7af5c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7af5c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7af5c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7af5c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7af5c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7af5c-113">Not supported.</span></span>    |
|<span data-ttu-id="7af5c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7af5c-114">Application</span></span> | <span data-ttu-id="7af5c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7af5c-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7af5c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7af5c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="7af5c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7af5c-117">Request headers</span></span>

| <span data-ttu-id="7af5c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7af5c-118">Header</span></span>       | <span data-ttu-id="7af5c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="7af5c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7af5c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7af5c-120">Authorization</span></span>  | <span data-ttu-id="7af5c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7af5c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7af5c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7af5c-123">Request body</span></span>

<span data-ttu-id="7af5c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7af5c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7af5c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7af5c-125">Response</span></span>

<span data-ttu-id="7af5c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7af5c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7af5c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7af5c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="7af5c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7af5c-129">Request</span></span>

<span data-ttu-id="7af5c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7af5c-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```

### <a name="response"></a><span data-ttu-id="7af5c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7af5c-131">Response</span></span>

<span data-ttu-id="7af5c-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7af5c-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp",
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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
