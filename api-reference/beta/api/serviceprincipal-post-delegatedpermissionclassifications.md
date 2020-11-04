---
title: Criar delegatedPermissionClassification
description: Classificar uma permissão adicionando um delegatedPermissionClassification à entidade de serviço da API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: d7cf0f78794910ec6ee5a19eadcb158c0fc8203e
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904774"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="2e442-103">Criar delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="2e442-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="2e442-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e442-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e442-105">Classificar uma permissão delegada adicionando um [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) ao [servicePrincipalName](../resources/servicePrincipal.md) que representa a API.</span><span class="sxs-lookup"><span data-stu-id="2e442-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e442-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e442-106">Permissions</span></span>

<span data-ttu-id="2e442-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e442-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e442-109">Permission type</span></span>      | <span data-ttu-id="2e442-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e442-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e442-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e442-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e442-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2e442-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="2e442-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e442-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e442-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e442-114">Not supported.</span></span>    |
|<span data-ttu-id="2e442-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e442-115">Application</span></span> | <span data-ttu-id="2e442-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2e442-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e442-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e442-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="2e442-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e442-118">Request headers</span></span>

| <span data-ttu-id="2e442-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2e442-119">Name</span></span>       | <span data-ttu-id="2e442-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e442-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="2e442-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e442-121">Authorization</span></span> | <span data-ttu-id="2e442-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e442-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2e442-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="2e442-124">Content-type</span></span> | <span data-ttu-id="2e442-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e442-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e442-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e442-127">Request body</span></span>

<span data-ttu-id="2e442-128">No corpo da solicitação, forneça uma representação JSON de um objeto [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) .</span><span class="sxs-lookup"><span data-stu-id="2e442-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2e442-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e442-129">Response</span></span>

<span data-ttu-id="2e442-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e442-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e442-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2e442-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e442-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e442-132">Request</span></span>

<span data-ttu-id="2e442-133">No exemplo a seguir, a permissão delegada "User. Read" está sendo classificada como "Low".</span><span class="sxs-lookup"><span data-stu-id="2e442-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>


# <a name="http"></a>[<span data-ttu-id="2e442-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e442-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="2e442-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e442-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2e442-136">C#</span><span class="sxs-lookup"><span data-stu-id="2e442-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-delegatedpermissionclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e442-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e442-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-delegatedpermissionclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e442-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e442-138">Response</span></span>

<span data-ttu-id="2e442-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e442-139">The following is an example of the response.</span></span>

> <span data-ttu-id="2e442-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e442-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "2G3-4TG6YU2J54hjnaRoPQE",
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
