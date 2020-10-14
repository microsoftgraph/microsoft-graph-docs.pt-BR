---
title: Criar permissionGrantConditionSet na coleção de inclusões de permissionGrantPolicy
description: Adicionar condições sob as quais um evento de concessão de permissão é incluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 0fdda1a2c3664df29ee12374d213366eda43856a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458679"
---
# <a name="create-permissiongrantconditionset-in-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="ff33a-103">Criar permissionGrantConditionSet na coleção de inclusões de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="ff33a-103">Create permissionGrantConditionSet in includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="ff33a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff33a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff33a-105">Adicionar condições sob as quais um evento de concessão de permissão é *incluído* em uma política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="ff33a-105">Add conditions under which a permission grant event is *included* in a permission grant policy.</span></span> <span data-ttu-id="ff33a-106">Para fazer isso, adicione um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) à coleção de **inclusões** de um  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ff33a-106">You do this by adding a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) to the **includes** collection of a  [permissionGrantPolicy](../resources/permissionGrantPolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff33a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff33a-107">Permissions</span></span>

<span data-ttu-id="ff33a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff33a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff33a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff33a-110">Permission type</span></span>      | <span data-ttu-id="ff33a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff33a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff33a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff33a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff33a-113">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ff33a-113">Policy.ReadWrite.PermissionGrant</span></span> |
|<span data-ttu-id="ff33a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff33a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff33a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff33a-115">Not supported.</span></span>    |
|<span data-ttu-id="ff33a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff33a-116">Application</span></span> | <span data-ttu-id="ff33a-117">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ff33a-117">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff33a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff33a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/permissionGrantPolicies/{id}/includes
```

## <a name="request-headers"></a><span data-ttu-id="ff33a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff33a-119">Request headers</span></span>

| <span data-ttu-id="ff33a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ff33a-120">Name</span></span>       | <span data-ttu-id="ff33a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff33a-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ff33a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff33a-122">Authorization</span></span> | <span data-ttu-id="ff33a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff33a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff33a-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="ff33a-125">Content-type</span></span> | <span data-ttu-id="ff33a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff33a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff33a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff33a-128">Request body</span></span>

<span data-ttu-id="ff33a-129">No corpo da solicitação, forneça uma representação JSON de um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) .</span><span class="sxs-lookup"><span data-stu-id="ff33a-129">In the request body, supply a JSON representation of an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ff33a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff33a-130">Response</span></span>

<span data-ttu-id="ff33a-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff33a-131">If successful, this method returns a `201 Created` response code and an [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff33a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff33a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff33a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff33a-133">Request</span></span>

<span data-ttu-id="ff33a-134">Neste exemplo, *todas* as permissões delegadas para aplicativos clientes de editores verificados estão incluídas na política de concessão de permissão.</span><span class="sxs-lookup"><span data-stu-id="ff33a-134">In this example, *all* delegated permissions for client apps from verified publishers are included in the permission grant policy.</span></span> <span data-ttu-id="ff33a-135">Como todas as outras condições do [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) foram omitidas, elas terão seus valores padrão, o que, em cada caso, é o mais inclusivo.</span><span class="sxs-lookup"><span data-stu-id="ff33a-135">Because all the other conditions from the [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) were omitted, they will take their default values, which in each case is the most-inclusive.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff33a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff33a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "permissiongrantpolicy_create_includes"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies/{id}/includes
Content-Type: application/json

{
  "permissionType": "delegated",
  "clientApplicationsFromVerifiedPublisherOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="ff33a-137">C#</span><span class="sxs-lookup"><span data-stu-id="ff33a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-create-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff33a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff33a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-create-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff33a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff33a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-create-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ff33a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff33a-140">Response</span></span>

<span data-ttu-id="ff33a-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff33a-141">The following is an example of the response.</span></span>

> <span data-ttu-id="ff33a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff33a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
