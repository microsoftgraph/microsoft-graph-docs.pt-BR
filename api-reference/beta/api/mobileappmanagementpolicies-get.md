---
title: Obter mobileAppManagementPolicy
description: Leia as propriedades e as relações de uma política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1e1e9bbd73ce8ac255673bc111e19fde3c69eb39
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442413"
---
# <a name="get-mobileappmanagementpolicy"></a><span data-ttu-id="d7fda-103">Obter mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="d7fda-103">Get mobileAppManagementPolicy</span></span>

<span data-ttu-id="d7fda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7fda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7fda-105">Leia as propriedades e as relações de um [objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d7fda-105">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7fda-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d7fda-106">Permissions</span></span>

<span data-ttu-id="d7fda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7fda-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7fda-109">Permission type</span></span>|<span data-ttu-id="d7fda-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7fda-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7fda-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7fda-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d7fda-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="d7fda-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="d7fda-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7fda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7fda-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7fda-114">Not supported.</span></span>|
|<span data-ttu-id="d7fda-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7fda-115">Application</span></span> | <span data-ttu-id="d7fda-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7fda-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7fda-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7fda-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d7fda-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7fda-118">Request headers</span></span>

|<span data-ttu-id="d7fda-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d7fda-119">Name</span></span>|<span data-ttu-id="d7fda-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7fda-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d7fda-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7fda-121">Authorization</span></span>|<span data-ttu-id="d7fda-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7fda-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7fda-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7fda-124">Request body</span></span>

<span data-ttu-id="d7fda-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7fda-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7fda-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7fda-126">Response</span></span>

<span data-ttu-id="d7fda-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7fda-127">If successful, this method returns a `200 OK` response code and a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7fda-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d7fda-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7fda-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7fda-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d7fda-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7fda-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```
# <a name="c"></a>[<span data-ttu-id="d7fda-131">C#</span><span class="sxs-lookup"><span data-stu-id="d7fda-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7fda-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7fda-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7fda-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7fda-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7fda-134">Java</span><span class="sxs-lookup"><span data-stu-id="d7fda-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7fda-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7fda-135">Response</span></span>

><span data-ttu-id="d7fda-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d7fda-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobilityManagementPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "ab90bacf-55a3-4a3e-839a-aa4b74e4f020",
    "appliesTo": "selected",
    "complianceUrl": "https://portal.mam.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.mam.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.mam.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
        "displayName": "Test Group"
      }
    ]
  }
}
```
