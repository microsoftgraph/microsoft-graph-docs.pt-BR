---
title: Excluir workforceIntegration
description: Excluir uma instância de um workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f44523533b40212a7735dc8ecbe70a7ec12666b4
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154056"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="ae67e-103">Excluir workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="ae67e-103">Delete workforceIntegration</span></span>

<span data-ttu-id="ae67e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae67e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae67e-105">Excluir uma instância de um [workforceIntegration](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="ae67e-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae67e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae67e-106">Permissions</span></span>

<span data-ttu-id="ae67e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae67e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae67e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae67e-109">Permission type</span></span>                        | <span data-ttu-id="ae67e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae67e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ae67e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae67e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae67e-112">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ae67e-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="ae67e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae67e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae67e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae67e-114">Not supported.</span></span> |
| <span data-ttu-id="ae67e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae67e-115">Application</span></span>                            | <span data-ttu-id="ae67e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae67e-116">Not supported.</span></span> |

> <span data-ttu-id="ae67e-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ae67e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ae67e-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="ae67e-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ae67e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae67e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="ae67e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae67e-120">Request headers</span></span>

| <span data-ttu-id="ae67e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ae67e-121">Name</span></span>          | <span data-ttu-id="ae67e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae67e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ae67e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae67e-123">Authorization</span></span> | <span data-ttu-id="ae67e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae67e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae67e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae67e-126">Request body</span></span>

<span data-ttu-id="ae67e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae67e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae67e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae67e-128">Response</span></span>

<span data-ttu-id="ae67e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae67e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae67e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ae67e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae67e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae67e-132">Request</span></span>

<span data-ttu-id="ae67e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae67e-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
```

---


### <a name="response"></a><span data-ttu-id="ae67e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae67e-134">Response</span></span>

<span data-ttu-id="ae67e-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae67e-135">The following is an example of the response.</span></span>

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
