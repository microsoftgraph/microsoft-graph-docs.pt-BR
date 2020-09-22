---
title: Atualizar um objeto connectedOrganization
description: Atualizar um objeto connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f7591a709065e42e9de87ea94873454512bbb0c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996472"
---
# <a name="update-connectedorganization"></a><span data-ttu-id="d6623-103">Atualizar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="d6623-103">Update connectedOrganization</span></span>

<span data-ttu-id="d6623-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6623-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6623-105">Atualize um objeto [connectedOrganization](../resources/connectedorganization.md) para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d6623-105">Update a [connectedOrganization](../resources/connectedorganization.md) object to change one or more of its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6623-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6623-106">Permissions</span></span>
<span data-ttu-id="d6623-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6623-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6623-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6623-109">Permission type</span></span>|<span data-ttu-id="d6623-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6623-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6623-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6623-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6623-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6623-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="d6623-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6623-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6623-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6623-114">Not supported.</span></span> |
|<span data-ttu-id="d6623-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6623-115">Application</span></span>                            | <span data-ttu-id="d6623-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6623-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6623-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6623-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d6623-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6623-118">Request headers</span></span>
|<span data-ttu-id="d6623-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d6623-119">Name</span></span>|<span data-ttu-id="d6623-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6623-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6623-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6623-121">Authorization</span></span>|<span data-ttu-id="d6623-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6623-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6623-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6623-124">Content-Type</span></span>|<span data-ttu-id="d6623-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6623-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6623-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6623-127">Request body</span></span>
<span data-ttu-id="d6623-128">No corpo da solicitação, forneça uma representação JSON do objeto [connectedOrganization](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="d6623-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="d6623-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar o [connectedOrganization](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="d6623-129">The following table shows the properties that are required when you update the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="d6623-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6623-130">Property</span></span>|<span data-ttu-id="d6623-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6623-131">Type</span></span>|<span data-ttu-id="d6623-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6623-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="d6623-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d6623-133">displayName</span></span>  |<span data-ttu-id="d6623-134">String</span><span class="sxs-lookup"><span data-stu-id="d6623-134">String</span></span> | <span data-ttu-id="d6623-135">O nome da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="d6623-135">The connected organization name.</span></span>  |
| <span data-ttu-id="d6623-136">description</span><span class="sxs-lookup"><span data-stu-id="d6623-136">description</span></span>  |<span data-ttu-id="d6623-137">String</span><span class="sxs-lookup"><span data-stu-id="d6623-137">String</span></span> | <span data-ttu-id="d6623-138">A descrição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="d6623-138">The connected organization description.</span></span> |
| <span data-ttu-id="d6623-139">state</span><span class="sxs-lookup"><span data-stu-id="d6623-139">state</span></span>        |<span data-ttu-id="d6623-140">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="d6623-140">connectedOrganizationState</span></span>|<span data-ttu-id="d6623-141">O estado de uma organização conectada define se as políticas de atribuição com tipo de escopo solicitante `AllConfiguredConnectedOrganizationSubjects` são aplicáveis ou não.</span><span class="sxs-lookup"><span data-stu-id="d6623-141">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="d6623-142">Os valores possíveis são: `configured` e `proposed`.</span><span class="sxs-lookup"><span data-stu-id="d6623-142">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="d6623-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6623-143">Response</span></span>

<span data-ttu-id="d6623-144">Se tiver êxito, este método retornará um `204 Accepted` código de resposta e um objeto [connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6623-144">If successful, this method returns a `204 Accepted` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6623-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d6623-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6623-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6623-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d6623-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6623-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectedorganization"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization new name",
  "description":"Connected organization new description",
  "state":"configured"
}
```
# <a name="c"></a>[<span data-ttu-id="d6623-148">C#</span><span class="sxs-lookup"><span data-stu-id="d6623-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6623-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6623-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6623-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6623-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d6623-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6623-151">Response</span></span>
<span data-ttu-id="d6623-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6623-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 204 Accepted
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization new name",
  "description":"Connected organization new description",
  "state":"configured"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


