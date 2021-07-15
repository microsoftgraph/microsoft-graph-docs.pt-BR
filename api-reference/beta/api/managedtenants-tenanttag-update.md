---
title: Atualizar tenantTag
description: Atualize as propriedades de um objeto tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 367fd71e769ae2fa4cd73b0f25f120b22fa5f0d9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442707"
---
# <a name="update-tenanttag"></a><span data-ttu-id="79314-103">Atualizar tenantTag</span><span class="sxs-lookup"><span data-stu-id="79314-103">Update tenantTag</span></span>
<span data-ttu-id="79314-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="79314-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79314-105">Atualize as propriedades de um [objeto tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="79314-105">Update the properties of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79314-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="79314-106">Permissions</span></span>
<span data-ttu-id="79314-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79314-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79314-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79314-109">Permission type</span></span>|<span data-ttu-id="79314-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79314-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79314-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79314-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79314-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="79314-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="79314-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79314-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79314-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79314-114">Not supported.</span></span>|
|<span data-ttu-id="79314-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79314-115">Application</span></span>|<span data-ttu-id="79314-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79314-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79314-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79314-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="79314-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79314-118">Request headers</span></span>
|<span data-ttu-id="79314-119">Nome</span><span class="sxs-lookup"><span data-stu-id="79314-119">Name</span></span>|<span data-ttu-id="79314-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="79314-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79314-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="79314-121">Authorization</span></span>|<span data-ttu-id="79314-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79314-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="79314-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79314-124">Content-Type</span></span>|<span data-ttu-id="79314-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79314-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79314-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79314-127">Request body</span></span>
<span data-ttu-id="79314-128">No corpo da solicitação, fornece os valores para campos [tenantTag](../resources/managedtenants-tenanttag.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="79314-128">In the request body, supply the values for relevant [tenantTag](../resources/managedtenants-tenanttag.md) fields that should be updated.</span></span> <span data-ttu-id="79314-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="79314-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="79314-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="79314-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="79314-131">As seguintes propriedades podem ser atualizadas:</span><span class="sxs-lookup"><span data-stu-id="79314-131">Following properties can be updated:</span></span>

| <span data-ttu-id="79314-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79314-132">Property</span></span>     | <span data-ttu-id="79314-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="79314-133">Type</span></span>        | <span data-ttu-id="79314-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="79314-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79314-135">displayName</span><span class="sxs-lookup"><span data-stu-id="79314-135">displayName</span></span>|<span data-ttu-id="79314-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79314-136">String</span></span>|<span data-ttu-id="79314-137">O nome de exibição da marca de locatário.</span><span class="sxs-lookup"><span data-stu-id="79314-137">The display name for the tenant tag.</span></span>|
|<span data-ttu-id="79314-138">description</span><span class="sxs-lookup"><span data-stu-id="79314-138">description</span></span>|<span data-ttu-id="79314-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79314-139">String</span></span>|<span data-ttu-id="79314-140">A descrição da marca de locatário.</span><span class="sxs-lookup"><span data-stu-id="79314-140">The description for the tenant tag.</span></span>|
|<span data-ttu-id="79314-141">locatários</span><span class="sxs-lookup"><span data-stu-id="79314-141">tenants</span></span>|<span data-ttu-id="79314-142">[coleção microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="79314-142">[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) collection</span></span>|<span data-ttu-id="79314-143">A coleção de locatários gerenciados associados à marca de locatário.</span><span class="sxs-lookup"><span data-stu-id="79314-143">The collection of managed tenants associated with the tenant tag.</span></span>|

## <a name="response"></a><span data-ttu-id="79314-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="79314-144">Response</span></span>

<span data-ttu-id="79314-145">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [tenantTag](../resources/managedtenants-tenanttag.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79314-145">If successful, this method returns a `200 OK` response code and an updated [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79314-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79314-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79314-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79314-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="79314-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="79314-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenanttag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
Content-Type: application/json
Content-length: 382

{
  "displayName": "Onboarding",
  "description": "Tenants that we are currently onboarding"
}
```
# <a name="c"></a>[<span data-ttu-id="79314-149">C#</span><span class="sxs-lookup"><span data-stu-id="79314-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79314-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79314-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79314-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79314-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79314-152">Java</span><span class="sxs-lookup"><span data-stu-id="79314-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79314-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="79314-153">Response</span></span>
><span data-ttu-id="79314-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="79314-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "913391c0-5466-42b4-900d-0a7501399cb0",
  "displayName": "Onboarding",
  "description": "Tenants that we are currently onboarding",
  "tenantIds": [
    {
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-16T20:36:31.086644Z",
  "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
  "lastActionDateTime": "2021-07-11T18:54:44.5262828Z",
  "lastActionByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0"
}
```
