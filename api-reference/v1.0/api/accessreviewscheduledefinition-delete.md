---
title: Excluir accessReviewScheduleDefinition
description: Exclui um objeto accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 697a762ec6234d14d55dfc7f345299dc071af2f1
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030992"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="7b474-103">Excluir accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="7b474-103">Delete accessReviewScheduleDefinition</span></span>
<span data-ttu-id="7b474-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b474-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b474-105">Exclui um [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7b474-105">Deletes an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b474-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b474-106">Permissions</span></span>
<span data-ttu-id="7b474-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b474-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b474-109">Permission type</span></span>|<span data-ttu-id="7b474-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b474-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b474-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b474-111">Delegated (work or school account)</span></span>| <span data-ttu-id="7b474-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b474-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="7b474-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b474-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b474-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b474-114">Not supported.</span></span>|
|<span data-ttu-id="7b474-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b474-115">Application</span></span>| <span data-ttu-id="7b474-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b474-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b474-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b474-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="7b474-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b474-118">Request headers</span></span>
|<span data-ttu-id="7b474-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7b474-119">Name</span></span>|<span data-ttu-id="7b474-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b474-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7b474-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b474-121">Authorization</span></span>|<span data-ttu-id="7b474-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b474-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b474-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b474-124">Request body</span></span>
<span data-ttu-id="7b474-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b474-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b474-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b474-126">Response</span></span>

<span data-ttu-id="7b474-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7b474-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7b474-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7b474-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b474-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b474-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessreviewscheduledefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```


### <a name="response"></a><span data-ttu-id="7b474-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b474-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
