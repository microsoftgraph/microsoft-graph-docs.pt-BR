---
title: Obter accessPackageAssignmentPolicy
description: Recupere as propriedades e os relacionamentos de um objeto accessPackageAassignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a0b3279188c4650efba4ae73cb7c1fccd4ae57ef
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935053"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="bb542-103">Obter accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="bb542-103">Get accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb542-104">No [Azure ad pretitulation Management](../resources/entitlementmanagement-root.md), recupere as propriedades e os relacionamentos de um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="bb542-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb542-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb542-105">Permissions</span></span>

<span data-ttu-id="bb542-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb542-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb542-108">Permission type</span></span>                        | <span data-ttu-id="bb542-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb542-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb542-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb542-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb542-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bb542-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="bb542-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb542-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb542-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb542-113">Not supported.</span></span> |
| <span data-ttu-id="bb542-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb542-114">Application</span></span>                            | <span data-ttu-id="bb542-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb542-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb542-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb542-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb542-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb542-117">Optional query parameters</span></span>

<span data-ttu-id="bb542-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb542-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bb542-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bb542-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb542-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb542-120">Request headers</span></span>

| <span data-ttu-id="bb542-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bb542-121">Name</span></span>      |<span data-ttu-id="bb542-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb542-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb542-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb542-123">Authorization</span></span> | <span data-ttu-id="bb542-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="bb542-124">Bearer \{token\}.</span></span> <span data-ttu-id="bb542-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb542-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb542-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb542-126">Request body</span></span>

<span data-ttu-id="bb542-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb542-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb542-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb542-128">Response</span></span>

<span data-ttu-id="bb542-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb542-129">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb542-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb542-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb542-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb542-131">Request</span></span>

<span data-ttu-id="bb542-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb542-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="bb542-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb542-133">Response</span></span>

<span data-ttu-id="bb542-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb542-134">The following is an example of the response.</span></span>

> <span data-ttu-id="bb542-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb542-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isEnabled": false,
  "canExtend": false,
  "durationInDays": 365
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
