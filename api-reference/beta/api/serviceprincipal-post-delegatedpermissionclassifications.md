---
title: Criar delegatedPermissionClassification
description: Classifique uma permissão adicionando um delegatedPermissionClassification à entidade de serviço da API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 7d286984628d52948593671137e9fecdf173da31
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050854"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="cd033-103">Criar delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="cd033-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="cd033-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd033-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd033-105">Classifique uma permissão delegada adicionando [uma delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) ao [servicePrincipal](../resources/servicePrincipal.md) que representa a API.</span><span class="sxs-lookup"><span data-stu-id="cd033-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd033-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd033-106">Permissions</span></span>

<span data-ttu-id="cd033-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd033-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd033-109">Permission type</span></span>      | <span data-ttu-id="cd033-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd033-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd033-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd033-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd033-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd033-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="cd033-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd033-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd033-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd033-114">Not supported.</span></span>    |
|<span data-ttu-id="cd033-115">Application</span><span class="sxs-lookup"><span data-stu-id="cd033-115">Application</span></span> | <span data-ttu-id="cd033-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd033-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd033-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd033-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="cd033-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd033-118">Request headers</span></span>

| <span data-ttu-id="cd033-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cd033-119">Name</span></span>       | <span data-ttu-id="cd033-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd033-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="cd033-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd033-121">Authorization</span></span> | <span data-ttu-id="cd033-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd033-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd033-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="cd033-124">Content-type</span></span> | <span data-ttu-id="cd033-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd033-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd033-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd033-127">Request body</span></span>

<span data-ttu-id="cd033-128">No corpo da solicitação, fornece uma representação JSON de um [objeto delegatedPermissionClassification.](../resources/delegatedpermissionclassification.md)</span><span class="sxs-lookup"><span data-stu-id="cd033-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cd033-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd033-129">Response</span></span>

<span data-ttu-id="cd033-130">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd033-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd033-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cd033-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd033-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd033-132">Request</span></span>

<span data-ttu-id="cd033-133">No exemplo a seguir, a permissão delegada "User.Read" está sendo classificada como "baixa".</span><span class="sxs-lookup"><span data-stu-id="cd033-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>


# <a name="http"></a>[<span data-ttu-id="cd033-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd033-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
# <a name="javascript"></a>[<span data-ttu-id="cd033-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd033-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cd033-136">C#</span><span class="sxs-lookup"><span data-stu-id="cd033-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-delegatedpermissionclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd033-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd033-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-delegatedpermissionclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd033-138">Java</span><span class="sxs-lookup"><span data-stu-id="cd033-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-delegatedpermissionclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd033-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd033-139">Response</span></span>

<span data-ttu-id="cd033-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd033-140">The following is an example of the response.</span></span>

> <span data-ttu-id="cd033-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cd033-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "2G3-4TG6YU2J54hjnaRoPQE",
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```

