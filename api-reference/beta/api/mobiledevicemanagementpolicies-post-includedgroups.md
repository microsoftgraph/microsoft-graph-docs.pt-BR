---
title: Adicionar includedGroups
description: Adicione grupos a serem incluídos em uma política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 08fd04903a13bed1515aa1a2ab313f79c4763d44
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440862"
---
# <a name="add-includedgroups"></a><span data-ttu-id="a4472-103">Adicionar includedGroups</span><span class="sxs-lookup"><span data-stu-id="a4472-103">Add includedGroups</span></span>

<span data-ttu-id="a4472-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4472-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4472-105">Adicione grupos a serem incluídos em uma política de gerenciamento de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="a4472-105">Add groups to be included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4472-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a4472-106">Permissions</span></span>

<span data-ttu-id="a4472-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4472-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4472-109">Permission type</span></span>|<span data-ttu-id="a4472-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4472-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4472-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4472-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4472-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="a4472-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="a4472-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4472-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4472-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4472-114">Not supported.</span></span>|
|<span data-ttu-id="a4472-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4472-115">Application</span></span> | <span data-ttu-id="a4472-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4472-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4472-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4472-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /policies/mobileDeviceManagementPolicies/{id}/includedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a4472-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4472-118">Request headers</span></span>
|<span data-ttu-id="a4472-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a4472-119">Name</span></span>|<span data-ttu-id="a4472-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4472-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4472-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4472-121">Authorization</span></span>|<span data-ttu-id="a4472-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4472-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a4472-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4472-124">Content-Type</span></span>|<span data-ttu-id="a4472-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4472-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4472-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4472-127">Request body</span></span>
<span data-ttu-id="a4472-128">No corpo da solicitação, fornece uma representação JSON do [objeto group.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="a4472-128">In the request body, supply a JSON representation of the [group](../resources/group.md) object.</span></span>

<span data-ttu-id="a4472-129">A tabela a seguir mostra as propriedades necessárias ao adicionar o [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="a4472-129">The following table shows the properties that are required when you add the [group](../resources/group.md).</span></span>

|<span data-ttu-id="a4472-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4472-130">Property</span></span>|<span data-ttu-id="a4472-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4472-131">Type</span></span>|<span data-ttu-id="a4472-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4472-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4472-133">id</span><span class="sxs-lookup"><span data-stu-id="a4472-133">id</span></span>|<span data-ttu-id="a4472-134">String</span><span class="sxs-lookup"><span data-stu-id="a4472-134">String</span></span>|<span data-ttu-id="a4472-135">O identificador exclusivo do grupo.</span><span class="sxs-lookup"><span data-stu-id="a4472-135">The unique identifier for the group.</span></span>|

## <a name="response"></a><span data-ttu-id="a4472-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4472-136">Response</span></span>

<span data-ttu-id="a4472-137">Se bem-sucedido, esse método retorna um código de resposta `204 No Content` e um objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4472-137">If successful, this method returns a `204 No Content` response code and a [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4472-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4472-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4472-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4472-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a4472-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4472-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef/includedGroups/$ref
Content-Type: application/json

{
  "@odata.id": "https://graph.microsoft.com/odata/groups('dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef')"
}
```
# <a name="c"></a>[<span data-ttu-id="a4472-141">C#</span><span class="sxs-lookup"><span data-stu-id="a4472-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-from-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4472-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4472-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-from-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4472-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4472-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-from-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4472-144">Java</span><span class="sxs-lookup"><span data-stu-id="a4472-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-from-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4472-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4472-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
