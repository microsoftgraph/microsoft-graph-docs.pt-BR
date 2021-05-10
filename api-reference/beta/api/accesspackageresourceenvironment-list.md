---
title: Listar accessPackageResourceEnvironments
description: Recupere uma lista de objetos accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4596ab46610f2e37c2103fe5aa334fb432386afc
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298123"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="a1d43-103">Listar accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="a1d43-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="a1d43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1d43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1d43-105">Recupere uma lista de [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="a1d43-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1d43-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1d43-106">Permissions</span></span>
<span data-ttu-id="a1d43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1d43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1d43-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1d43-109">Permission type</span></span>|<span data-ttu-id="a1d43-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1d43-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1d43-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1d43-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1d43-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1d43-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="a1d43-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1d43-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1d43-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a1d43-114">Not supported</span></span>|
|<span data-ttu-id="a1d43-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1d43-115">Application</span></span>|<span data-ttu-id="a1d43-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a1d43-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1d43-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d43-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1d43-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1d43-118">Optional query parameters</span></span>
<span data-ttu-id="a1d43-119">Este método requer o parâmetro `$filter` [de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a1d43-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="a1d43-120">Você deve aplicar `$filter` a um **originSystem** definido como ( `eq` ) `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="a1d43-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1d43-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d43-121">Request headers</span></span>
|<span data-ttu-id="a1d43-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a1d43-122">Name</span></span>|<span data-ttu-id="a1d43-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1d43-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a1d43-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1d43-124">Authorization</span></span>|<span data-ttu-id="a1d43-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1d43-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1d43-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d43-127">Request body</span></span>
<span data-ttu-id="a1d43-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1d43-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1d43-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d43-129">Response</span></span>

<span data-ttu-id="a1d43-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1d43-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1d43-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1d43-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1d43-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1d43-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a1d43-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1d43-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```
# <a name="c"></a>[<span data-ttu-id="a1d43-134">C#</span><span class="sxs-lookup"><span data-stu-id="a1d43-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1d43-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1d43-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1d43-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1d43-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1d43-137">Java</span><span class="sxs-lookup"><span data-stu-id="a1d43-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a1d43-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1d43-138">Response</span></span>
> <span data-ttu-id="a1d43-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1d43-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageResourceEnvironment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments",
  "value": [
    {
      "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
      "displayName": "https://contoso.sharepoint.com/",
      "description": "https://contoso.sharepoint.com/",
      "originSystem": "SharePointOnline",
      "originId": "https://contoso-admin.sharepoint.com/",
      "isDefaultEnvironment": false,
      "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
      }
    }
  ]
}
```

