---
title: Criar accessPackageAssignmentRequest
description: Criar um novo accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06fe6ed015a7aa9e6d90a473e89750be058b236f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442023"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="780cb-103">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="780cb-103">Create accessPackageAssignmentRequest</span></span>

<span data-ttu-id="780cb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="780cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="780cb-105">Em [Gerenciamento de qualificação do Azure ad](../resources/entitlementmanagement-root.md), crie um novo objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="780cb-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="780cb-106">Essa operação é usada para atribuir um usuário a um pacote do Access ou para remover uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="780cb-106">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="780cb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="780cb-107">Permissions</span></span>

<span data-ttu-id="780cb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="780cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="780cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="780cb-110">Permission type</span></span>                        | <span data-ttu-id="780cb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="780cb-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="780cb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="780cb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="780cb-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="780cb-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="780cb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="780cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="780cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="780cb-115">Not supported.</span></span> |
| <span data-ttu-id="780cb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="780cb-116">Application</span></span>                            | <span data-ttu-id="780cb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="780cb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="780cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="780cb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="780cb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="780cb-119">Request headers</span></span>

| <span data-ttu-id="780cb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="780cb-120">Name</span></span>          | <span data-ttu-id="780cb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="780cb-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="780cb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="780cb-122">Authorization</span></span> | <span data-ttu-id="780cb-123">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="780cb-123">Bearer \{token\}.</span></span> <span data-ttu-id="780cb-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="780cb-124">Required.</span></span> |
| <span data-ttu-id="780cb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="780cb-125">Content-Type</span></span>  | <span data-ttu-id="780cb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="780cb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="780cb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="780cb-128">Request body</span></span>

<span data-ttu-id="780cb-129">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="780cb-129">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="780cb-130">Para criar uma atribuição para um usuário, o valor da propriedade **RequestType** é `AdminAdd`, e a propriedade **accessPackageAssignment** contém o `targetId` do usuário que está sendo atribuído, a propriedade **assignmentPolicyId** que identifica o [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)e a propriedade **accessPackageId** identificando o [accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="780cb-130">To create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="780cb-131">Para remover uma atribuição, o valor da propriedade **RequestType** é `AdminRemove`, e a propriedade **accessPackageAssignment** contém a propriedade **ID** que identifica o [accessPackageAssignment](../resources/accesspackageassignment.md) que está sendo removido.</span><span class="sxs-lookup"><span data-stu-id="780cb-131">To remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

## <a name="response"></a><span data-ttu-id="780cb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="780cb-132">Response</span></span>

<span data-ttu-id="780cb-133">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="780cb-133">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="780cb-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="780cb-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="780cb-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="780cb-135">Request</span></span>

<span data-ttu-id="780cb-136">Veja a seguir um exemplo da solicitação de uma atribuição direta.</span><span class="sxs-lookup"><span data-stu-id="780cb-136">The following is an example of the request for a direct assignment.</span></span>  <span data-ttu-id="780cb-137">O valor de **TargetId** é a ID de objeto de um usuário que está sendo atribuído, o valor do **accessPackageId** é o pacote de acesso desejado e o valor de **assignmentPolicyId** é uma política de atribuição direta no pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="780cb-137">The value of the **targetID** is the object ID of a user being assigned, the value of the **accessPackageId** is the desired access package, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="780cb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="780cb-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="780cb-139">C#</span><span class="sxs-lookup"><span data-stu-id="780cb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="780cb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="780cb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="780cb-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="780cb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="780cb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="780cb-142">Response</span></span>

<span data-ttu-id="780cb-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="780cb-143">The following is an example of the response.</span></span>

> <span data-ttu-id="780cb-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="780cb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
