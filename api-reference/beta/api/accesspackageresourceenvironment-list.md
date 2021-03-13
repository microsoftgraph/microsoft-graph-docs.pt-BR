---
title: Listar accessPackageResourceEnvironments
description: Recupere uma lista de objetos accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 823abc8a71cfce4ac7872f4e6e86ae7d08e92411
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759402"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="2b08b-103">Listar accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="2b08b-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="2b08b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b08b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b08b-105">Recupere uma lista de [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="2b08b-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b08b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b08b-106">Permissions</span></span>
<span data-ttu-id="2b08b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b08b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b08b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b08b-109">Permission type</span></span>|<span data-ttu-id="2b08b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b08b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b08b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b08b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b08b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b08b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="2b08b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b08b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b08b-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2b08b-114">Not supported</span></span>|
|<span data-ttu-id="2b08b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b08b-115">Application</span></span>|<span data-ttu-id="2b08b-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2b08b-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b08b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b08b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b08b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2b08b-118">Optional query parameters</span></span>
<span data-ttu-id="2b08b-119">Este método requer o parâmetro `$filter` [de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2b08b-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="2b08b-120">Você deve aplicar `$filter` a um **originSystem** definido como ( `eq` ) `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="2b08b-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b08b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b08b-121">Request headers</span></span>
|<span data-ttu-id="2b08b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2b08b-122">Name</span></span>|<span data-ttu-id="2b08b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b08b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b08b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b08b-124">Authorization</span></span>|<span data-ttu-id="2b08b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b08b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b08b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b08b-127">Request body</span></span>
<span data-ttu-id="2b08b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b08b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b08b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b08b-129">Response</span></span>

<span data-ttu-id="2b08b-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b08b-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b08b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2b08b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b08b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b08b-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2b08b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b08b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```
# <a name="c"></a>[<span data-ttu-id="2b08b-134">C#</span><span class="sxs-lookup"><span data-stu-id="2b08b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b08b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b08b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b08b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b08b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b08b-137">Java</span><span class="sxs-lookup"><span data-stu-id="2b08b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2b08b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b08b-138">Response</span></span>
<span data-ttu-id="2b08b-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2b08b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

