---
title: Criar accessPackageAssignmentPolicy
description: Use esta API para criar um novo accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 280a532c2d0047fecb0085f88b73c92c30a4867f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935047"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="ab797-103">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="ab797-103">Create accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab797-104">No [Gerenciamento de qualificação do Azure ad](../resources/entitlementmanagement-root.md), use esta API para criar um novo objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ab797-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), use this API to create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab797-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab797-105">Permissions</span></span>

<span data-ttu-id="ab797-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab797-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab797-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab797-108">Permission type</span></span>                        | <span data-ttu-id="ab797-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab797-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab797-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab797-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab797-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab797-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="ab797-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab797-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab797-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab797-113">Not supported.</span></span> |
| <span data-ttu-id="ab797-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab797-114">Application</span></span>                            | <span data-ttu-id="ab797-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab797-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab797-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab797-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="ab797-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab797-117">Request headers</span></span>

| <span data-ttu-id="ab797-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ab797-118">Name</span></span>          | <span data-ttu-id="ab797-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab797-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ab797-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab797-120">Authorization</span></span> | <span data-ttu-id="ab797-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="ab797-121">Bearer \{token\}.</span></span> <span data-ttu-id="ab797-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab797-122">Required.</span></span> |
| <span data-ttu-id="ab797-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab797-123">Content-Type</span></span>  | <span data-ttu-id="ab797-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab797-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab797-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab797-125">Request body</span></span>

<span data-ttu-id="ab797-126">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ab797-126">In the request body, supply a JSON representation of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ab797-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab797-127">Response</span></span>

<span data-ttu-id="ab797-128">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab797-128">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab797-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab797-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab797-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab797-130">Request</span></span>

<span data-ttu-id="ab797-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab797-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "isEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="ab797-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab797-132">Response</span></span>

<span data-ttu-id="ab797-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab797-133">The following is an example of the response.</span></span>

> <span data-ttu-id="ab797-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab797-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
