---
title: Listar accessPackageResourceEnvironments
description: Recupere uma lista de objetos accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf7116ef1512dca40cae66d92030b032d3aefa23
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137689"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="b8f27-103">Listar accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="b8f27-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="b8f27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8f27-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8f27-105">Recupere uma lista de [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b8f27-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8f27-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8f27-106">Permissions</span></span>
<span data-ttu-id="b8f27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8f27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8f27-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8f27-109">Permission type</span></span>|<span data-ttu-id="b8f27-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8f27-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8f27-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8f27-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8f27-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8f27-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="b8f27-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8f27-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8f27-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8f27-114">Not supported</span></span>|
|<span data-ttu-id="b8f27-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8f27-115">Application</span></span>|<span data-ttu-id="b8f27-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8f27-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8f27-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8f27-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8f27-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8f27-118">Optional query parameters</span></span>
<span data-ttu-id="b8f27-119">Esse método requer o parâmetro `$filter` [de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b8f27-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="b8f27-120">Você deve aplicar `$filter` a um **originSystem** definido como ( `eq` ) `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="b8f27-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8f27-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f27-121">Request headers</span></span>
|<span data-ttu-id="b8f27-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b8f27-122">Name</span></span>|<span data-ttu-id="b8f27-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8f27-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b8f27-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8f27-124">Authorization</span></span>|<span data-ttu-id="b8f27-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8f27-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8f27-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f27-127">Request body</span></span>
<span data-ttu-id="b8f27-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8f27-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8f27-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8f27-129">Response</span></span>

<span data-ttu-id="b8f27-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8f27-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8f27-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8f27-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8f27-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f27-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```


### <a name="response"></a><span data-ttu-id="b8f27-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8f27-133">Response</span></span>
<span data-ttu-id="b8f27-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8f27-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

