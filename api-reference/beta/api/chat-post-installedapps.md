---
title: Adicionar o aplicativo ao chat
description: Instalar um aplicativo para chat.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ce4e7c8bee2535840b2d0f3d6fb234fb38ffbaf2
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607458"
---
# <a name="add-app-to-chat"></a><span data-ttu-id="e2233-103">Adicionar o aplicativo ao chat</span><span class="sxs-lookup"><span data-stu-id="e2233-103">Add app to chat</span></span>

<span data-ttu-id="e2233-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2233-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2233-105">Instale um [teamsApp](../resources/teamsapp.md) para o [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="e2233-105">Install a [teamsApp](../resources/teamsapp.md) to the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e2233-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e2233-106">Permissions</span></span>

<span data-ttu-id="e2233-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2233-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2233-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2233-109">Permission type</span></span>      | <span data-ttu-id="e2233-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2233-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2233-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2233-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e2233-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="e2233-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="e2233-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2233-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2233-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2233-114">Not supported.</span></span>    |
|<span data-ttu-id="e2233-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2233-115">Application</span></span> | <span data-ttu-id="e2233-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="e2233-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2233-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2233-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
POST /chats/{chat-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="e2233-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2233-118">Request headers</span></span>

| <span data-ttu-id="e2233-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2233-119">Header</span></span>       | <span data-ttu-id="e2233-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e2233-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e2233-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2233-121">Authorization</span></span>  | <span data-ttu-id="e2233-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2233-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2233-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2233-124">Content-Type</span></span>  | <span data-ttu-id="e2233-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2233-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2233-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2233-127">Request body</span></span>

<span data-ttu-id="e2233-128">O corpo da solicitação deve conter a ID do aplicativo gerado pelo aplicativo de catálogo.</span><span class="sxs-lookup"><span data-stu-id="e2233-128">The request body should contain the catalog app's generated app ID.</span></span> <span data-ttu-id="e2233-129">Para obter detalhes, confira [teamsApp Properties](../resources/teamsapp.md#properties).</span><span class="sxs-lookup"><span data-stu-id="e2233-129">For details, see [teamsApp properties](../resources/teamsapp.md#properties).</span></span>

## <a name="response"></a><span data-ttu-id="e2233-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2233-130">Response</span></span>

<span data-ttu-id="e2233-131">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="e2233-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e2233-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e2233-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2233-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2233-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "add_app_in_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps
Content-Type: application/json

{
"teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="e2233-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2233-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation"
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat add installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
