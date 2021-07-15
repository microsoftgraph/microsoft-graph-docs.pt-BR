---
title: 'tenantGroup: tenantSearch'
description: Pesquisa os locatários gerenciados especificados entre grupos de locatários.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 73cf4f28cfa22bd0f881bc1d00c91aa8c0b2cf03
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441796"
---
# <a name="tenantgroup-tenantsearch"></a><span data-ttu-id="b39eb-103">tenantGroup: tenantSearch</span><span class="sxs-lookup"><span data-stu-id="b39eb-103">tenantGroup: tenantSearch</span></span>
<span data-ttu-id="b39eb-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="b39eb-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b39eb-105">Pesquisa os locatários gerenciados especificados entre grupos de locatários.</span><span class="sxs-lookup"><span data-stu-id="b39eb-105">Searches for the specified managed tenants across tenant groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="b39eb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b39eb-106">Permissions</span></span>
<span data-ttu-id="b39eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b39eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b39eb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b39eb-109">Permission type</span></span>|<span data-ttu-id="b39eb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b39eb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b39eb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b39eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b39eb-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b39eb-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="b39eb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b39eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b39eb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b39eb-114">Not supported.</span></span>|
|<span data-ttu-id="b39eb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b39eb-115">Application</span></span>|<span data-ttu-id="b39eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b39eb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b39eb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b39eb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantGroups/tenantSearch
```

## <a name="request-headers"></a><span data-ttu-id="b39eb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b39eb-118">Request headers</span></span>
|<span data-ttu-id="b39eb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b39eb-119">Name</span></span>|<span data-ttu-id="b39eb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b39eb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b39eb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b39eb-121">Authorization</span></span>|<span data-ttu-id="b39eb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b39eb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b39eb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b39eb-124">Content-Type</span></span>|<span data-ttu-id="b39eb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b39eb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b39eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b39eb-127">Request body</span></span>
<span data-ttu-id="b39eb-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b39eb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b39eb-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b39eb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b39eb-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b39eb-130">Parameter</span></span>|<span data-ttu-id="b39eb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b39eb-131">Type</span></span>|<span data-ttu-id="b39eb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b39eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b39eb-133">tenantId</span><span class="sxs-lookup"><span data-stu-id="b39eb-133">tenantId</span></span>|<span data-ttu-id="b39eb-134">String</span><span class="sxs-lookup"><span data-stu-id="b39eb-134">String</span></span>|<span data-ttu-id="b39eb-135">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="b39eb-135">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|



## <a name="response"></a><span data-ttu-id="b39eb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b39eb-136">Response</span></span>

<span data-ttu-id="b39eb-137">Se tiver êxito, essa ação retornará um código de resposta e uma `200 OK` [coleção microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b39eb-137">If successful, this action returns a `200 OK` response code and a [microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b39eb-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b39eb-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b39eb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b39eb-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b39eb-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b39eb-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenantgroup_tenantsearch"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantGroups/tenantSearch
Content-Type: application/json
Content-length: 28

{
  "tenantId": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="b39eb-141">C#</span><span class="sxs-lookup"><span data-stu-id="b39eb-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenantgroup-tenantsearch-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b39eb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b39eb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenantgroup-tenantsearch-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b39eb-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b39eb-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenantgroup-tenantsearch-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b39eb-144">Java</span><span class="sxs-lookup"><span data-stu-id="b39eb-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenantgroup-tenantsearch-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b39eb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b39eb-145">Response</span></span>
><span data-ttu-id="b39eb-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b39eb-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantGroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantGroups",
  "value": [
    {
      "id": "2e6a0c9f-986d-480e-ad4b-bdfddc047aba",
      "displayName": "Default",
      "allTenantsIncluded": true,
      "tenantIds": [],
      "managementIntents": [
        {
          "managementIntentId": "586895ab-8a59-4b79-be25-b06949a819bb",
          "managementIntentDisplayName": "Default Baseline",
          "managementTemplates": [
            {
              "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
              "displayName": "Baseline - Block Legacy Authentication",
              "category": "identity"
            },
            {
              "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
              "displayName": "Baseline - Require MFA for Admins",
              "category": "identity"
            },
            {
              "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
              "displayName": "Baseline - Require MFA for end users",
              "category": "identity"
            },
            {
              "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
              "displayName": "Baseline - Enroll devices in MEM",
              "category": "devices"
            },
            {
              "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
              "displayName": "Baseline - Setup Compliance Policy for Windows 10 devices",
              "category": "devices"
            },
            {
              "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
              "displayName": "Baseline - Setup Microsoft Defender Antivirus Policy for Windows 10 devices",
              "category": "devices"
            }
          ]
        }
      ],
      "managementActions": []
    }
  ]
}
```
