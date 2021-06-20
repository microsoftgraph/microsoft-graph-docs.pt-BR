---
title: 'accessReviewInstance: sendReminder'
description: Envia um lembrete aos revisores de um accessReviewInstance ativo no momento.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8e47c8cb68d1cba3d6933dd62d68d930deb6b0bb
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030997"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="46803-103">accessReviewInstance: sendReminder</span><span class="sxs-lookup"><span data-stu-id="46803-103">accessReviewInstance: sendReminder</span></span>
<span data-ttu-id="46803-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46803-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46803-105">Envie um lembrete aos revisores de um [accessReviewInstance ativo.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="46803-105">Send a reminder to the reviewers of an active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="46803-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46803-106">Permissions</span></span>
<span data-ttu-id="46803-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46803-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46803-109">Permission type</span></span>|<span data-ttu-id="46803-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46803-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46803-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46803-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46803-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46803-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="46803-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46803-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46803-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46803-114">Not supported.</span></span>|
|<span data-ttu-id="46803-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46803-115">Application</span></span>|<span data-ttu-id="46803-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46803-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46803-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46803-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/sendReminder
```

## <a name="request-headers"></a><span data-ttu-id="46803-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46803-118">Request headers</span></span>
|<span data-ttu-id="46803-119">Nome</span><span class="sxs-lookup"><span data-stu-id="46803-119">Name</span></span>|<span data-ttu-id="46803-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="46803-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46803-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="46803-121">Authorization</span></span>|<span data-ttu-id="46803-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46803-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46803-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46803-124">Request body</span></span>
<span data-ttu-id="46803-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46803-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46803-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="46803-126">Response</span></span>

<span data-ttu-id="46803-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46803-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="46803-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46803-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46803-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46803-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_sendreminder"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/sendReminder
```


### <a name="response"></a><span data-ttu-id="46803-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="46803-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
