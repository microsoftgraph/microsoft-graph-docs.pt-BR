---
title: Criar connectedOrganization
description: Criar um novo connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 47e8ba9564b1810da99e212ab9832142656d18f0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509936"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="a6d5e-103">Criar connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="a6d5e-103">Create connectedOrganization</span></span>

<span data-ttu-id="a6d5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6d5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6d5e-105">Criar um novo objeto [connectedOrganization](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="a6d5e-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6d5e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6d5e-106">Permissions</span></span>

<span data-ttu-id="a6d5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6d5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6d5e-109">Permission type</span></span>|<span data-ttu-id="a6d5e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6d5e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="a6d5e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6d5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6d5e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6d5e-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a6d5e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6d5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6d5e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-114">Not supported.</span></span> |
| <span data-ttu-id="a6d5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6d5e-115">Application</span></span>                            | <span data-ttu-id="a6d5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6d5e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6d5e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="a6d5e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6d5e-118">Request headers</span></span>

|<span data-ttu-id="a6d5e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a6d5e-119">Name</span></span>|<span data-ttu-id="a6d5e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6d5e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a6d5e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6d5e-121">Authorization</span></span>|<span data-ttu-id="a6d5e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a6d5e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6d5e-124">Content-Type</span></span>|<span data-ttu-id="a6d5e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6d5e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6d5e-127">Request body</span></span>
<span data-ttu-id="a6d5e-128">No corpo da solicitação, forneça uma representação JSON do objeto [connectedOrganization](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="a6d5e-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="a6d5e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [connectedOrganization](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="a6d5e-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="a6d5e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6d5e-130">Property</span></span>|<span data-ttu-id="a6d5e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6d5e-131">Type</span></span>|<span data-ttu-id="a6d5e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6d5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6d5e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a6d5e-133">displayName</span></span>|<span data-ttu-id="a6d5e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6d5e-134">String</span></span>|<span data-ttu-id="a6d5e-135">O nome da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-135">The connected organization name.</span></span> |
|<span data-ttu-id="a6d5e-136">description</span><span class="sxs-lookup"><span data-stu-id="a6d5e-136">description</span></span>|<span data-ttu-id="a6d5e-137">String</span><span class="sxs-lookup"><span data-stu-id="a6d5e-137">String</span></span>|<span data-ttu-id="a6d5e-138">A descrição da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-138">The connected organization description.</span></span>|
|<span data-ttu-id="a6d5e-139">identitySources</span><span class="sxs-lookup"><span data-stu-id="a6d5e-139">identitySources</span></span>|<span data-ttu-id="a6d5e-140">coleção [identityry](../resources/identitysource.md)</span><span class="sxs-lookup"><span data-stu-id="a6d5e-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="a6d5e-141">Uma coleção com um elemento, a fonte de identidade inicial nesta organização conectada.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-141">A collection with one element, the initial identity source in this connected organization.</span></span>|


## <a name="response"></a><span data-ttu-id="a6d5e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6d5e-142">Response</span></span>

<span data-ttu-id="a6d5e-143">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-143">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6d5e-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a6d5e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6d5e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6d5e-145">Request</span></span>
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="a6d5e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6d5e-146">Response</span></span>
<span data-ttu-id="a6d5e-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a6d5e-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "modifiedDateTime": "2020-06-08T20:13:53.7099947Z"
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
