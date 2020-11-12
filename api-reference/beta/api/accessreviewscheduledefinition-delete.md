---
title: Excluir accessReviewScheduleDefinition
description: Excluir um objeto accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d72e5321cf74e66bd34e48b4d6000715f11ea09d
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000726"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="437f4-103">Excluir accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="437f4-103">Delete accessReviewScheduleDefinition</span></span>

<span data-ttu-id="437f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="437f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="437f4-105">Excluir um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="437f4-105">Delete an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="437f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="437f4-106">Permissions</span></span>
<span data-ttu-id="437f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="437f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="437f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="437f4-109">Permission type</span></span>                        | <span data-ttu-id="437f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="437f4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="437f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="437f4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="437f4-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="437f4-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="437f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="437f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="437f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="437f4-114">Not supported.</span></span>|
|<span data-ttu-id="437f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="437f4-115">Application</span></span>                            | <span data-ttu-id="437f4-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="437f4-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="437f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="437f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="437f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="437f4-118">Request headers</span></span>
<span data-ttu-id="437f4-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="437f4-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="437f4-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="437f4-120">Request body</span></span>
<span data-ttu-id="437f4-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="437f4-121">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="437f4-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="437f4-122">Response</span></span>
<span data-ttu-id="437f4-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="437f4-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="437f4-125">Exemplos</span><span class="sxs-lookup"><span data-stu-id="437f4-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="437f4-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="437f4-126">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/29f2d16e-9ca6-4052-bbfe-802c48981fd8
```

---

### <a name="response"></a><span data-ttu-id="437f4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="437f4-127">Response</span></span>
><span data-ttu-id="437f4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="437f4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
