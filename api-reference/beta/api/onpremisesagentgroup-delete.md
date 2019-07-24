---
title: Excluir onPremisesAgentGroup
description: Excluir um objeto **onPremisesAgentGroup** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f893502156560e455dbed46a1db4e9dc6faf327
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841161"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="bb38a-103">Excluir onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="bb38a-103">Delete onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb38a-104">Excluir um objeto [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="bb38a-104">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb38a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb38a-105">Permissions</span></span>

<span data-ttu-id="bb38a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb38a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb38a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb38a-108">Permission type</span></span>                        | <span data-ttu-id="bb38a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb38a-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb38a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb38a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb38a-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bb38a-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="bb38a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb38a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb38a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb38a-113">Not supported.</span></span> |
| <span data-ttu-id="bb38a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb38a-114">Application</span></span>                            | <span data-ttu-id="bb38a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb38a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb38a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb38a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="bb38a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb38a-117">Request headers</span></span>

| <span data-ttu-id="bb38a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bb38a-118">Name</span></span>          | <span data-ttu-id="bb38a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb38a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bb38a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb38a-120">Authorization</span></span> | <span data-ttu-id="bb38a-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="bb38a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb38a-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb38a-122">Request body</span></span>

<span data-ttu-id="bb38a-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb38a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb38a-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb38a-124">Response</span></span>

<span data-ttu-id="bb38a-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb38a-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb38a-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb38a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb38a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb38a-128">Request</span></span>

<span data-ttu-id="bb38a-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb38a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```

### <a name="response"></a><span data-ttu-id="bb38a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb38a-130">Response</span></span>

<span data-ttu-id="bb38a-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb38a-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
