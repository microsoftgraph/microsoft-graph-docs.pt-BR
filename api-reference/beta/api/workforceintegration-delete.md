---
title: Excluir workforceIntegration
description: Excluir uma instância de um workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 01e690c517e0f8b84b1f059ba153d4bb9de7026e
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895522"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="2386b-103">Excluir workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="2386b-103">Delete workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2386b-104">Excluir uma instância de um [workforceIntegration](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="2386b-104">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2386b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2386b-105">Permissions</span></span>

<span data-ttu-id="2386b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2386b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2386b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2386b-108">Permission type</span></span>                        | <span data-ttu-id="2386b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2386b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2386b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2386b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2386b-111">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2386b-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="2386b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2386b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2386b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2386b-113">Not supported.</span></span> |
| <span data-ttu-id="2386b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2386b-114">Application</span></span>                            | <span data-ttu-id="2386b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2386b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2386b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2386b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="2386b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2386b-117">Request headers</span></span>

| <span data-ttu-id="2386b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2386b-118">Name</span></span>          | <span data-ttu-id="2386b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2386b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2386b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2386b-120">Authorization</span></span> | <span data-ttu-id="2386b-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2386b-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2386b-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2386b-122">Request body</span></span>

<span data-ttu-id="2386b-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2386b-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2386b-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="2386b-124">Response</span></span>

<span data-ttu-id="2386b-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2386b-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2386b-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2386b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2386b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2386b-128">Request</span></span>

<span data-ttu-id="2386b-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2386b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```

### <a name="response"></a><span data-ttu-id="2386b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2386b-130">Response</span></span>

<span data-ttu-id="2386b-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2386b-131">The following is an example of the response.</span></span>

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
  "description": "Delete workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->