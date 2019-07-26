---
title: 'teamsAppInstallation: atualização'
description: Atualizar uma instalação de aplicativo no escopo pessoal de um usuário
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7461c6e320ffcacc0d26ccffe90681ab6215db15
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908534"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="d3f4f-103">teamsAppInstallation: atualização</span><span class="sxs-lookup"><span data-stu-id="d3f4f-103">teamsAppInstallation: upgrade</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3f4f-104">Atualize uma [instalação de aplicativo](../resources/teamsappinstallation.md) no escopo pessoal do [usuário](../resources/user.md) especificado para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-104">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3f4f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3f4f-105">Permissions</span></span>

<span data-ttu-id="d3f4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f4f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3f4f-108">Permission type</span></span>      | <span data-ttu-id="d3f4f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3f4f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3f4f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3f4f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3f4f-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3f4f-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="d3f4f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3f4f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3f4f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-113">Not supported.</span></span>    |
|<span data-ttu-id="d3f4f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3f4f-114">Application</span></span> | <span data-ttu-id="d3f4f-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3f4f-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3f4f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3f4f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="d3f4f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f4f-117">Request headers</span></span>

| <span data-ttu-id="d3f4f-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3f4f-118">Header</span></span>       | <span data-ttu-id="d3f4f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="d3f4f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3f4f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3f4f-120">Authorization</span></span>  | <span data-ttu-id="d3f4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3f4f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f4f-123">Request body</span></span>

<span data-ttu-id="d3f4f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3f4f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3f4f-125">Response</span></span>

<span data-ttu-id="d3f4f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f4f-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3f4f-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3f4f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3f4f-129">Request</span></span>

<span data-ttu-id="d3f4f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

### <a name="response"></a><span data-ttu-id="d3f4f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3f4f-131">Response</span></span>

<span data-ttu-id="d3f4f-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "user_upgrade_teamsApp",
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
  "description": "Upgrade teamsApp for user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
