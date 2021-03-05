---
title: Criar permissionGrantConditionSet em inclui coleção de permissionGrantPolicy
description: Adicione condições em que um evento de concessão de permissão está incluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 1300319e2411a7e5e39b7cf9d1fd5ad365a2f363
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448072"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="eb950-103">Criar permissionGrantConditionSet em inclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="eb950-103">Create permissionGrantConditionSet in includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="eb950-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb950-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb950-105">Adicione condições em que um evento de concessão de permissão *está incluído* em uma política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="eb950-105">Add conditions under which a permission grant event is *included* in a permission grant policy.</span></span> <span data-ttu-id="eb950-106">Você faz isso adicionando [uma permissionGrantConditionSet](../resources/permissiongrantconditionset.md) à coleção **includes** de  [uma permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="eb950-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **includes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb950-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb950-107">Permissions</span></span>

<span data-ttu-id="eb950-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb950-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb950-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb950-110">Permission type</span></span>      | <span data-ttu-id="eb950-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb950-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb950-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb950-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb950-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="eb950-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="eb950-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb950-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb950-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb950-115">Not supported.</span></span>    |
|<span data-ttu-id="eb950-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb950-116">Application</span></span> | <span data-ttu-id="eb950-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="eb950-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb950-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb950-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/includes
```

## <a name="request-headers"></a><span data-ttu-id="eb950-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb950-119">Request headers</span></span>

| <span data-ttu-id="eb950-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eb950-120">Name</span></span>       | <span data-ttu-id="eb950-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb950-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="eb950-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb950-122">Authorization</span></span> | <span data-ttu-id="eb950-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb950-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb950-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="eb950-125">Content-type</span></span> | <span data-ttu-id="eb950-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb950-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb950-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb950-128">Request body</span></span>

<span data-ttu-id="eb950-129">No corpo da solicitação, fornece uma representação JSON de [um objeto permissionGrantConditionSet.](../resources/permissiongrantconditionset.md)</span><span class="sxs-lookup"><span data-stu-id="eb950-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eb950-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb950-130">Response</span></span>

<span data-ttu-id="eb950-131">Se tiver êxito, este método retornará um código de `201 Created` resposta e um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb950-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb950-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb950-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb950-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb950-133">Request</span></span>

<span data-ttu-id="eb950-134">Neste exemplo, *todas as* permissões delegadas para aplicativos cliente de editores verificados são incluídas na política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="eb950-134">In this example, *all* delegated permissions for client apps from verified publishers are included in the permission grant policy.</span></span> <span data-ttu-id="eb950-135">Como todas as outras condições do [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) foram omitidas, elas aceitarão seus valores padrão, que, em cada caso, são os mais inclusivos.</span><span class="sxs-lookup"><span data-stu-id="eb950-135">Because all the other conditions from the [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) were omitted, they will take their default values, which in each case is the most-inclusive.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb950-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb950-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_includes"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/{id}/includes
Content-Type: application/json

{
  "permissionType": "delegated",
  "clientApplicationsFromVerifiedPublisherOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="eb950-137">C#</span><span class="sxs-lookup"><span data-stu-id="eb950-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb950-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb950-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb950-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb950-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb950-140">Java</span><span class="sxs-lookup"><span data-stu-id="eb950-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-create-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb950-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb950-141">Response</span></span>

<span data-ttu-id="eb950-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb950-142">The following is an example of the response.</span></span>

> <span data-ttu-id="eb950-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb950-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "75ffda85-9314-43bc-bf19-554a7d079e96",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "any",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
