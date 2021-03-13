---
title: Obter aprovação
description: Recupere as propriedades de um objeto de aprovação.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9f2a3c1d32d578937a6d124da73136292958cfc
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760748"
---
# <a name="get-approval"></a><span data-ttu-id="5b772-103">Obter aprovação</span><span class="sxs-lookup"><span data-stu-id="5b772-103">Get approval</span></span>

<span data-ttu-id="5b772-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b772-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b772-105">Recupere as propriedades de um [objeto de aprovação.](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="5b772-105">Retrieve the properties of an [approval](../resources/approval.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b772-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b772-106">Permissions</span></span>

<span data-ttu-id="5b772-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b772-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b772-109">Permission type</span></span>                        | <span data-ttu-id="5b772-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b772-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5b772-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b772-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b772-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b772-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5b772-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b772-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b772-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b772-114">Not supported.</span></span> |
| <span data-ttu-id="5b772-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b772-115">Application</span></span>                            | <span data-ttu-id="5b772-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b772-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b772-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b772-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5b772-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b772-118">Request headers</span></span>

| <span data-ttu-id="5b772-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5b772-119">Name</span></span>      |<span data-ttu-id="5b772-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b772-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b772-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b772-121">Authorization</span></span> | <span data-ttu-id="5b772-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="5b772-122">Bearer \{token\}.</span></span> <span data-ttu-id="5b772-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b772-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b772-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b772-124">Request body</span></span>

<span data-ttu-id="5b772-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b772-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b772-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b772-126">Response</span></span>

<span data-ttu-id="5b772-127">Se tiver êxito, este método retornará um código de resposta e o objeto de aprovação `200 OK` solicitado no corpo da resposta. [](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="5b772-127">If successful, this method returns a `200 OK` response code and the requested [approval](../resources/approval.md) object in the response body.</span></span> <span data-ttu-id="5b772-128">No entanto, se o chamador não tiver as permissões certas, o método retornará um `403 Forbidden` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b772-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5b772-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b772-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b772-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b772-130">Request</span></span>

<span data-ttu-id="5b772-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b772-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_approval"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489
```
---


### <a name="response"></a><span data-ttu-id="5b772-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b772-132">Response</span></span>

<span data-ttu-id="5b772-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b772-133">The following is an example of the response.</span></span>

> <span data-ttu-id="5b772-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b772-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approval"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "abd306ef-f7b2-4a10-9fd1-493454322489",
    "steps": [
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
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


