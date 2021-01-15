---
title: Criar connectedOrganization
description: Crie uma nova connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75981889ae018e3c5852dae52bcb6ac09a195103
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872678"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="31061-103">Criar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="31061-103">Create connectedOrganization</span></span>

<span data-ttu-id="31061-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31061-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31061-105">Crie um novo [objeto connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="31061-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31061-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31061-106">Permissions</span></span>

<span data-ttu-id="31061-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31061-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31061-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31061-109">Permission type</span></span>|<span data-ttu-id="31061-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31061-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="31061-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31061-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="31061-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31061-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="31061-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31061-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31061-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31061-114">Not supported.</span></span> |
| <span data-ttu-id="31061-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31061-115">Application</span></span>                            | <span data-ttu-id="31061-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31061-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31061-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31061-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="31061-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31061-118">Request headers</span></span>

|<span data-ttu-id="31061-119">Nome</span><span class="sxs-lookup"><span data-stu-id="31061-119">Name</span></span>|<span data-ttu-id="31061-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="31061-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="31061-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="31061-121">Authorization</span></span>|<span data-ttu-id="31061-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31061-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="31061-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31061-124">Content-Type</span></span>|<span data-ttu-id="31061-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31061-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31061-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31061-127">Request body</span></span>
<span data-ttu-id="31061-128">No corpo da solicitação, fornece uma representação JSON do [objeto connectedOrganization](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="31061-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="31061-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [connectedOrganization](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="31061-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="31061-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31061-130">Property</span></span>|<span data-ttu-id="31061-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31061-131">Type</span></span>|<span data-ttu-id="31061-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31061-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31061-133">displayName</span><span class="sxs-lookup"><span data-stu-id="31061-133">displayName</span></span>|<span data-ttu-id="31061-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31061-134">String</span></span>|<span data-ttu-id="31061-135">O nome da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="31061-135">The connected organization name.</span></span> |
|<span data-ttu-id="31061-136">description</span><span class="sxs-lookup"><span data-stu-id="31061-136">description</span></span>|<span data-ttu-id="31061-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31061-137">String</span></span>|<span data-ttu-id="31061-138">A descrição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="31061-138">The connected organization description.</span></span>|
|<span data-ttu-id="31061-139">identitySources</span><span class="sxs-lookup"><span data-stu-id="31061-139">identitySources</span></span>|<span data-ttu-id="31061-140">[Coleção identitySource](../resources/identitysource.md)</span><span class="sxs-lookup"><span data-stu-id="31061-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="31061-141">Uma coleção com um elemento, a fonte de identidade inicial nesta organização conectada.</span><span class="sxs-lookup"><span data-stu-id="31061-141">A collection with one element, the initial identity source in this connected organization.</span></span>|
|<span data-ttu-id="31061-142">state</span><span class="sxs-lookup"><span data-stu-id="31061-142">state</span></span>|<span data-ttu-id="31061-143">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="31061-143">connectedOrganizationState</span></span>|<span data-ttu-id="31061-144">O estado de uma organização conectada define se as políticas de atribuição com o tipo de escopo do solicitante `AllConfiguredConnectedOrganizationSubjects` são aplicáveis ou não.</span><span class="sxs-lookup"><span data-stu-id="31061-144">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="31061-145">Os valores possíveis são: `configured` e `proposed`.</span><span class="sxs-lookup"><span data-stu-id="31061-145">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="31061-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="31061-146">Response</span></span>

<span data-ttu-id="31061-147">Se bem-sucedido, este método retorna um código de resposta e um novo objeto `201 Created` [connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31061-147">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31061-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31061-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31061-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31061-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="31061-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="31061-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectedorganization_from_connectedorganizations"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.domainIdentitySource",
      "domainName": "example.com",
      "displayName": "example.com"
      }
  ],
  "state":"proposed"
}
```
# <a name="c"></a>[<span data-ttu-id="31061-151">C#</span><span class="sxs-lookup"><span data-stu-id="31061-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectedorganization-from-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31061-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31061-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectedorganization-from-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31061-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31061-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectedorganization-from-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31061-154">Java</span><span class="sxs-lookup"><span data-stu-id="31061-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectedorganization-from-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31061-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="31061-155">Response</span></span>
<span data-ttu-id="31061-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31061-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-06-08T20:13:53.7099947Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-06-08T20:13:53.7099947Z",
  "state":"proposed"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


