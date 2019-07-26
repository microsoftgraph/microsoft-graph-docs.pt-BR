---
title: Remover aplicativo da equipe
description: Desinstala um aplicativo da equipe especificada.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 149b905a6e090960351ae0da70b2a6080fea8fa1
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908470"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="55807-103">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="55807-103">Remove app from team</span></span>

<span data-ttu-id="55807-104">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="55807-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="55807-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="55807-105">Permissions</span></span>

<span data-ttu-id="55807-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55807-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55807-108">Permission type</span></span>      | <span data-ttu-id="55807-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55807-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55807-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55807-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55807-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55807-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="55807-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55807-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55807-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55807-113">Not supported.</span></span>    |
|<span data-ttu-id="55807-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55807-114">Application</span></span> | <span data-ttu-id="55807-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55807-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="55807-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55807-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="55807-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55807-117">Request headers</span></span>

| <span data-ttu-id="55807-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55807-118">Header</span></span>       | <span data-ttu-id="55807-119">Valor</span><span class="sxs-lookup"><span data-stu-id="55807-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55807-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="55807-120">Authorization</span></span>  | <span data-ttu-id="55807-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55807-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55807-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55807-123">Request body</span></span>

<span data-ttu-id="55807-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55807-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55807-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="55807-125">Response</span></span>

<span data-ttu-id="55807-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55807-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55807-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55807-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="55807-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55807-129">Request</span></span>

<span data-ttu-id="55807-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55807-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->

```http
DELETE /teams/{id}/installedApps/{id}
```

### <a name="response"></a><span data-ttu-id="55807-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="55807-131">Response</span></span>

<span data-ttu-id="55807-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55807-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
