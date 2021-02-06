---
title: Acessar AccessPackageResourceEnvironment
description: Leia as propriedades e os relacionamentos de um objeto accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ec973b1f8d7b38b27e267d54b8cbcd424af23bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137687"
---
# <a name="get-accesspackageresourceenvironment"></a><span data-ttu-id="533f3-103">Acessar AccessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="533f3-103">Get accessPackageResourceEnvironment</span></span>
<span data-ttu-id="533f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="533f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="533f3-105">Leia as propriedades e os relacionamentos de um [objeto accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="533f3-105">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="533f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="533f3-106">Permissions</span></span>
<span data-ttu-id="533f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="533f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="533f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="533f3-109">Permission type</span></span>|<span data-ttu-id="533f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="533f3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="533f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="533f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="533f3-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="533f3-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="533f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="533f3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="533f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="533f3-114">Not supported.</span></span>|
|<span data-ttu-id="533f3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="533f3-115">Application</span></span>|<span data-ttu-id="533f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="533f3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="533f3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="533f3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="533f3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="533f3-118">Optional query parameters</span></span>
<span data-ttu-id="533f3-119">No momento, esse método não dá suporte [a parâmetros de consulta OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="533f3-119">This method does not currently support [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="533f3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="533f3-120">Request headers</span></span>
|<span data-ttu-id="533f3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="533f3-121">Name</span></span>|<span data-ttu-id="533f3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="533f3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="533f3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="533f3-123">Authorization</span></span>|<span data-ttu-id="533f3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="533f3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="533f3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="533f3-126">Request body</span></span>
<span data-ttu-id="533f3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="533f3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="533f3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="533f3-128">Response</span></span>

<span data-ttu-id="533f3-129">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` [objeto accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="533f3-129">If successful, this method returns a `200 OK` response code and an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="533f3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="533f3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="533f3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="533f3-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```


### <a name="response"></a><span data-ttu-id="533f3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="533f3-132">Response</span></span>
<span data-ttu-id="533f3-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="533f3-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

