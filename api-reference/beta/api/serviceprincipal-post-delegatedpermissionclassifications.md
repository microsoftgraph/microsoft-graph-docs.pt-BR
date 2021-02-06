---
title: Criar delegatedPermissionClassification
description: Classifique uma permissão adicionando um delegatedPermissionClassification à entidade de serviço da API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 631c68bb6986362c5c9743dd59b2d51809d5bbfb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134187"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="dd4ab-103">Criar delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="dd4ab-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="dd4ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd4ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd4ab-105">Classifique uma permissão delegada adicionando [uma delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) à [servicePrincipal](../resources/servicePrincipal.md) que representa a API.</span><span class="sxs-lookup"><span data-stu-id="dd4ab-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd4ab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd4ab-106">Permissions</span></span>

<span data-ttu-id="dd4ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd4ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd4ab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd4ab-109">Permission type</span></span>      | <span data-ttu-id="dd4ab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd4ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd4ab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd4ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd4ab-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd4ab-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="dd4ab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd4ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd4ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd4ab-114">Not supported.</span></span>    |
|<span data-ttu-id="dd4ab-115">Application</span><span class="sxs-lookup"><span data-stu-id="dd4ab-115">Application</span></span> | <span data-ttu-id="dd4ab-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd4ab-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd4ab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd4ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="dd4ab-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd4ab-118">Request headers</span></span>

| <span data-ttu-id="dd4ab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dd4ab-119">Name</span></span>       | <span data-ttu-id="dd4ab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd4ab-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="dd4ab-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd4ab-121">Authorization</span></span> | <span data-ttu-id="dd4ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd4ab-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dd4ab-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="dd4ab-124">Content-type</span></span> | <span data-ttu-id="dd4ab-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd4ab-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd4ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd4ab-127">Request body</span></span>

<span data-ttu-id="dd4ab-128">No corpo da solicitação, fornece uma representação JSON de [um objeto delegatedPermissionClassification.](../resources/delegatedpermissionclassification.md)</span><span class="sxs-lookup"><span data-stu-id="dd4ab-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dd4ab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd4ab-129">Response</span></span>

<span data-ttu-id="dd4ab-130">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd4ab-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd4ab-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dd4ab-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd4ab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd4ab-132">Request</span></span>

<span data-ttu-id="dd4ab-133">No exemplo a seguir, a permissão delegada "User.Read" está sendo classificada como "baixa".</span><span class="sxs-lookup"><span data-stu-id="dd4ab-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>


# <a name="http"></a>[<span data-ttu-id="dd4ab-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd4ab-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="dd4ab-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd4ab-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="dd4ab-136">C#</span><span class="sxs-lookup"><span data-stu-id="dd4ab-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-delegatedpermissionclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd4ab-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd4ab-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-delegatedpermissionclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd4ab-138">Java</span><span class="sxs-lookup"><span data-stu-id="dd4ab-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-delegatedpermissionclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd4ab-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd4ab-139">Response</span></span>

<span data-ttu-id="dd4ab-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd4ab-140">The following is an example of the response.</span></span>

> <span data-ttu-id="dd4ab-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd4ab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

