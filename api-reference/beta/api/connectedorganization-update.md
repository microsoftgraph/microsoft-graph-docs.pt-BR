---
title: Atualizar um objeto connectedOrganization
description: Atualizar um objeto connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f8e45830d9f8c970b97d142029505cd61185b36
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957558"
---
# <a name="update-connectedorganization"></a><span data-ttu-id="527e3-103">Atualizar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="527e3-103">Update connectedOrganization</span></span>

<span data-ttu-id="527e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="527e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="527e3-105">Atualize um objeto [connectedOrganization](../resources/connectedorganization.md) para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="527e3-105">Update a [connectedOrganization](../resources/connectedorganization.md) object to change one or more of its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="527e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="527e3-106">Permissions</span></span>
<span data-ttu-id="527e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="527e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="527e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="527e3-109">Permission type</span></span>|<span data-ttu-id="527e3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="527e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="527e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="527e3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="527e3-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="527e3-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="527e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="527e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="527e3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="527e3-114">Not supported.</span></span> |
|<span data-ttu-id="527e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="527e3-115">Application</span></span>                            | <span data-ttu-id="527e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="527e3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="527e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="527e3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="527e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="527e3-118">Request headers</span></span>
|<span data-ttu-id="527e3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="527e3-119">Name</span></span>|<span data-ttu-id="527e3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="527e3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="527e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="527e3-121">Authorization</span></span>|<span data-ttu-id="527e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="527e3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="527e3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="527e3-124">Content-Type</span></span>|<span data-ttu-id="527e3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="527e3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="527e3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="527e3-127">Request body</span></span>
<span data-ttu-id="527e3-128">No corpo da solicitação, forneça uma representação JSON do objeto [connectedOrganization](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="527e3-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="527e3-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar o [connectedOrganization](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="527e3-129">The following table shows the properties that are required when you update the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="527e3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="527e3-130">Property</span></span>|<span data-ttu-id="527e3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="527e3-131">Type</span></span>|<span data-ttu-id="527e3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="527e3-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="527e3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="527e3-133">displayName</span></span>  |<span data-ttu-id="527e3-134">String</span><span class="sxs-lookup"><span data-stu-id="527e3-134">String</span></span> | <span data-ttu-id="527e3-135">O nome da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="527e3-135">The connected organization name.</span></span>  |
| <span data-ttu-id="527e3-136">description</span><span class="sxs-lookup"><span data-stu-id="527e3-136">description</span></span>  |<span data-ttu-id="527e3-137">String</span><span class="sxs-lookup"><span data-stu-id="527e3-137">String</span></span> | <span data-ttu-id="527e3-138">A descrição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="527e3-138">The connected organization description.</span></span> |
| <span data-ttu-id="527e3-139">state</span><span class="sxs-lookup"><span data-stu-id="527e3-139">state</span></span>        |<span data-ttu-id="527e3-140">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="527e3-140">connectedOrganizationState</span></span>|<span data-ttu-id="527e3-141">O estado de uma organização conectada define se as políticas de atribuição com tipo de escopo solicitante `AllConfiguredConnectedOrganizationSubjects` são aplicáveis ou não.</span><span class="sxs-lookup"><span data-stu-id="527e3-141">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="527e3-142">Os valores possíveis são: `configured` e `proposed`.</span><span class="sxs-lookup"><span data-stu-id="527e3-142">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="527e3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="527e3-143">Response</span></span>

<span data-ttu-id="527e3-144">Se tiver êxito, este método retornará um `204 Accepted` código de resposta e um objeto [connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="527e3-144">If successful, this method returns a `204 Accepted` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="527e3-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="527e3-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="527e3-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="527e3-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="527e3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="527e3-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="527e3-148">C#</span><span class="sxs-lookup"><span data-stu-id="527e3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="527e3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="527e3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="527e3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="527e3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="527e3-151">Java</span><span class="sxs-lookup"><span data-stu-id="527e3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="527e3-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="527e3-152">Response</span></span>
<span data-ttu-id="527e3-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="527e3-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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


