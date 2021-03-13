---
title: Obter approvalStep
description: Recupere as propriedades de um objeto approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e4de431a5fca9321d2b60f4a3a978d5cb40fb973
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760747"
---
# <a name="get-approvalstep"></a><span data-ttu-id="5a983-103">Obter approvalStep</span><span class="sxs-lookup"><span data-stu-id="5a983-103">Get approvalStep</span></span>

<span data-ttu-id="5a983-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a983-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a983-105">Recupere as propriedades de um [objeto approvalStep.](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="5a983-105">Retrieve the properties of an [approvalStep](../resources/approvalstep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a983-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a983-106">Permissions</span></span>

<span data-ttu-id="5a983-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a983-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a983-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a983-109">Permission type</span></span>                        | <span data-ttu-id="5a983-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a983-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5a983-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a983-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a983-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a983-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5a983-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a983-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a983-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a983-114">Not supported.</span></span> |
| <span data-ttu-id="5a983-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a983-115">Application</span></span>                            | <span data-ttu-id="5a983-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a983-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a983-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a983-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5a983-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a983-118">Request headers</span></span>

| <span data-ttu-id="5a983-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5a983-119">Name</span></span>      |<span data-ttu-id="5a983-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a983-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a983-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a983-121">Authorization</span></span> | <span data-ttu-id="5a983-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="5a983-122">Bearer \{token\}.</span></span> <span data-ttu-id="5a983-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a983-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a983-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a983-124">Request body</span></span>

<span data-ttu-id="5a983-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a983-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a983-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a983-126">Response</span></span>

<span data-ttu-id="5a983-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [approvalStep](../resources/approvalstep.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a983-127">If successful, this method returns a `200 OK` response code and the [approvalStep](../resources/approvalstep.md) object in the response body.</span></span> <span data-ttu-id="5a983-128">No entanto, se o chamador não tiver as permissões certas, o método retornará um `403 Forbidden` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a983-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5a983-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5a983-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a983-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a983-130">Request</span></span>

<span data-ttu-id="5a983-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a983-131">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_approvalstep"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
---


### <a name="response"></a><span data-ttu-id="5a983-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a983-132">Response</span></span>

<span data-ttu-id="5a983-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a983-133">The following is an example of the response.</span></span>

> <span data-ttu-id="5a983-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a983-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d4fa4045-4716-436d-aec5-57b0a713f095",
    "displayName": null,
    "reviewedDateTime": null,
    "reviewResult": "NotReviewed",
    "status": "InProgress",
    "assignedToMe": true,
    "justification": "",
    "reviewedBy": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


