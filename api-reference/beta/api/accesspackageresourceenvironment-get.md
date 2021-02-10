---
title: Acessar AccessPackageResourceEnvironment
description: Leia as propriedades e os relacionamentos de um objeto accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0169ad18a24ff27392c5679f91dfaecd43d76567
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176273"
---
# <a name="get-accesspackageresourceenvironment"></a><span data-ttu-id="6283a-103">Acessar AccessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="6283a-103">Get accessPackageResourceEnvironment</span></span>
<span data-ttu-id="6283a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6283a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6283a-105">Leia as propriedades e os relacionamentos de um [objeto accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="6283a-105">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6283a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6283a-106">Permissions</span></span>
<span data-ttu-id="6283a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6283a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6283a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6283a-109">Permission type</span></span>|<span data-ttu-id="6283a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6283a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6283a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6283a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6283a-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6283a-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="6283a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6283a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6283a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6283a-114">Not supported.</span></span>|
|<span data-ttu-id="6283a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6283a-115">Application</span></span>|<span data-ttu-id="6283a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6283a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6283a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6283a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6283a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6283a-118">Optional query parameters</span></span>
<span data-ttu-id="6283a-119">No momento, esse método não dá suporte [a parâmetros de consulta OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="6283a-119">This method does not currently support [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6283a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6283a-120">Request headers</span></span>
|<span data-ttu-id="6283a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6283a-121">Name</span></span>|<span data-ttu-id="6283a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6283a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6283a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6283a-123">Authorization</span></span>|<span data-ttu-id="6283a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6283a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6283a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6283a-126">Request body</span></span>
<span data-ttu-id="6283a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6283a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6283a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6283a-128">Response</span></span>

<span data-ttu-id="6283a-129">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6283a-129">If successful, this method returns a `200 OK` response code and an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6283a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6283a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6283a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6283a-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6283a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6283a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```
# <a name="c"></a>[<span data-ttu-id="6283a-133">C#</span><span class="sxs-lookup"><span data-stu-id="6283a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6283a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6283a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6283a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6283a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6283a-136">Java</span><span class="sxs-lookup"><span data-stu-id="6283a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6283a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6283a-137">Response</span></span>
<span data-ttu-id="6283a-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6283a-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments/$entity",
    "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
    "displayName": "https://contoso.sharepoint.com/",
    "description": "GeoLocation: , RootSiteUrl: https://contoso.sharepoint.com/, TenantAdminUrl: https://contoso-admin.sharepoint.com/",
    "originSystem": "SharePointOnline",
    "originId": "https://contoso-admin.sharepoint.com/",
    "isDefaultEnvironment": false,
    "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
    }
}
```

