---
title: Criar permissionGrantConditionSet em exclui coleção de permissionGrantPolicy
description: Adicione condições nas quais um evento de concessão de permissão é excluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: a15b82fdc595da0a032b2d6962cdcf02b57843fc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433912"
---
# <a name="create-permissiongrantconditionset-in-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="1b6cb-103">Criar permissionGrantConditionSet em exclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="1b6cb-103">Create permissionGrantConditionSet in excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="1b6cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b6cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b6cb-105">Adicione condições nas quais um evento de concessão de permissão *é excluído* em uma política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="1b6cb-105">Add conditions under which a permission grant event is *excluded* in a permission grant policy.</span></span> <span data-ttu-id="1b6cb-106">Você faz isso adicionando [uma permissionGrantConditionSet](../resources/permissiongrantconditionset.md) à coleção **excludes** de  [uma permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1b6cb-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **excludes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b6cb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b6cb-107">Permissions</span></span>

<span data-ttu-id="1b6cb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b6cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b6cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b6cb-110">Permission type</span></span>      | <span data-ttu-id="1b6cb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b6cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b6cb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b6cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b6cb-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1b6cb-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="1b6cb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b6cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b6cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b6cb-115">Not supported.</span></span>    |
|<span data-ttu-id="1b6cb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b6cb-116">Application</span></span> | <span data-ttu-id="1b6cb-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1b6cb-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b6cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b6cb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="request-headers"></a><span data-ttu-id="1b6cb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6cb-119">Request headers</span></span>

| <span data-ttu-id="1b6cb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1b6cb-120">Name</span></span>       | <span data-ttu-id="1b6cb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b6cb-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="1b6cb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b6cb-122">Authorization</span></span> | <span data-ttu-id="1b6cb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b6cb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b6cb-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="1b6cb-125">Content-type</span></span> | <span data-ttu-id="1b6cb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b6cb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b6cb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6cb-128">Request body</span></span>

<span data-ttu-id="1b6cb-129">No corpo da solicitação, fornece uma representação JSON de [um objeto permissionGrantConditionSet.](../resources/permissiongrantconditionset.md)</span><span class="sxs-lookup"><span data-stu-id="1b6cb-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1b6cb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b6cb-130">Response</span></span>

<span data-ttu-id="1b6cb-131">Se tiver êxito, este método retornará um código de `201 Created` resposta e um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b6cb-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b6cb-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b6cb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b6cb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6cb-133">Request</span></span>

<span data-ttu-id="1b6cb-134">Neste *exemplo,* todas as permissões delegadas para o Microsoft Graph (**appId** 000000003-0000-0000-c000-000000000000) são excluídas da política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="1b6cb-134">In this example, *all* delegated permissions for Microsoft Graph (**appId** 00000003-0000-0000-c000-000000000000) are excluded from the permission grant policy.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b6cb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b6cb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_excludes"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/excludes
Content-Type: application/json

{
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="1b6cb-136">C#</span><span class="sxs-lookup"><span data-stu-id="1b6cb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b6cb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b6cb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b6cb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b6cb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b6cb-139">Java</span><span class="sxs-lookup"><span data-stu-id="1b6cb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-create-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b6cb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b6cb-140">Response</span></span>

<span data-ttu-id="1b6cb-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b6cb-141">The following is an example of the response.</span></span>

> <span data-ttu-id="1b6cb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b6cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "9a532f49-e646-405d-8c7c-d4c8e8a4d294",
  "permissionClassification": "all",
  "permissionType": "delegated",
  "resourceApplication": "00000003-0000-0000-c000-000000000000",
  "permissions": ["all"],
  "clientApplicationIds": ["all"],
  "clientApplicationTenantIds": ["all"],
  "clientApplicationPublisherIds": ["all"],
  "clientApplicationsFromVerifiedPublisherOnly": false
}
```
