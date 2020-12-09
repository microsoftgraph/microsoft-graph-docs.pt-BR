---
title: 'teamsAppInstallation: atualização'
description: Atualizar uma instalação de aplicativo no escopo pessoal de um usuário
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 661cf87471fbfe3ab16dbc47334ce6487f60b51f
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607296"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="309b9-103">teamsAppInstallation: atualização</span><span class="sxs-lookup"><span data-stu-id="309b9-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="309b9-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="309b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="309b9-105">Atualize uma [instalação de aplicativo](../resources/teamsappinstallation.md) no escopo pessoal do [usuário](../resources/user.md) especificado para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="309b9-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="309b9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="309b9-106">Permissions</span></span>

<span data-ttu-id="309b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="309b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="309b9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="309b9-109">Permission type</span></span>      | <span data-ttu-id="309b9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="309b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="309b9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="309b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="309b9-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="309b9-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="309b9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="309b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="309b9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="309b9-114">Not supported.</span></span>    |
|<span data-ttu-id="309b9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="309b9-115">Application</span></span> | <span data-ttu-id="309b9-116">TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All</span><span class="sxs-lookup"><span data-stu-id="309b9-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="309b9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="309b9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id}/teamwork/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="309b9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="309b9-118">Request headers</span></span>

| <span data-ttu-id="309b9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="309b9-119">Header</span></span>       | <span data-ttu-id="309b9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="309b9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="309b9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="309b9-121">Authorization</span></span>  | <span data-ttu-id="309b9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="309b9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="309b9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="309b9-124">Request body</span></span>

<span data-ttu-id="309b9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="309b9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="309b9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="309b9-126">Response</span></span>

<span data-ttu-id="309b9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="309b9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="309b9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="309b9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="309b9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="309b9-130">Request</span></span>

<span data-ttu-id="309b9-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="309b9-131">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->

```http
POST /users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk/upgrade
```

### <a name="response"></a><span data-ttu-id="309b9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="309b9-132">Response</span></span>

<span data-ttu-id="309b9-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="309b9-133">The following is an example of the response.</span></span>

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
