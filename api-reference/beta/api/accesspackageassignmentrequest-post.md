---
title: Criar accessPackageAssignmentRequest
description: Criar um novo accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90530cb12ece487c440fee2f1283dec787cda709
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935037"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="22f3c-103">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="22f3c-103">Create accessPackageAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22f3c-104">Em [Gerenciamento de qualificação do Azure ad](../resources/entitlementmanagement-root.md), crie um novo objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="22f3c-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22f3c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="22f3c-105">Permissions</span></span>

<span data-ttu-id="22f3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22f3c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22f3c-108">Permission type</span></span>                        | <span data-ttu-id="22f3c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22f3c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22f3c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22f3c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="22f3c-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="22f3c-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="22f3c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22f3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22f3c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22f3c-113">Not supported.</span></span> |
| <span data-ttu-id="22f3c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22f3c-114">Application</span></span>                            | <span data-ttu-id="22f3c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22f3c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22f3c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22f3c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="22f3c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22f3c-117">Request headers</span></span>

| <span data-ttu-id="22f3c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="22f3c-118">Name</span></span>          | <span data-ttu-id="22f3c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="22f3c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="22f3c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="22f3c-120">Authorization</span></span> | <span data-ttu-id="22f3c-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="22f3c-121">Bearer \{token\}.</span></span> <span data-ttu-id="22f3c-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22f3c-122">Required.</span></span> |
| <span data-ttu-id="22f3c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22f3c-123">Content-Type</span></span>  | <span data-ttu-id="22f3c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="22f3c-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22f3c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22f3c-125">Request body</span></span>

<span data-ttu-id="22f3c-126">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="22f3c-126">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="22f3c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f3c-127">Response</span></span>

<span data-ttu-id="22f3c-128">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22f3c-128">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22f3c-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22f3c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22f3c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22f3c-130">Request</span></span>

<span data-ttu-id="22f3c-131">Veja a seguir um exemplo da solicitação de uma atribuição direta.</span><span class="sxs-lookup"><span data-stu-id="22f3c-131">The following is an example of the request for a direct assignment.</span></span>  <span data-ttu-id="22f3c-132">O valor de `targetID` é a ID de objeto de um usuário que está sendo atribuído, o valor `accessPackageId` do é o pacote de acesso desejado e o valor `assignmentPolicyId` de é uma política de atribuição direta no pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="22f3c-132">The value of the `targetID` is the object ID of a user being assigned, the value of the `accessPackageId` is the desired access package, and the value of `assignmentPolicyId` is a direct assignment policy in that access package.</span></span>
 
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```

### <a name="response"></a><span data-ttu-id="22f3c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f3c-133">Response</span></span>

<span data-ttu-id="22f3c-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22f3c-134">The following is an example of the response.</span></span>

> <span data-ttu-id="22f3c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22f3c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->