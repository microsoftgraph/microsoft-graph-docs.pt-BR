---
title: Listar accessPackageResourceRoles
description: Recupere uma lista de objetos accessPackageResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 184b5f25321c0c87270a6c1616233b913de31298
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441981"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="9be4a-103">Listar accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="9be4a-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="9be4a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9be4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9be4a-105">Recupere uma lista de objetos [accessPackageResourceRole](../resources/accesspackageresourcerole.md) de um [AccessPackageResource](../resources/accesspackageresource.md) em um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="9be4a-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="9be4a-106">Essa lista de funções pode ser usada pelo chamador para selecionar uma função, que é necessária ao [criar um accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span><span class="sxs-lookup"><span data-stu-id="9be4a-106">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9be4a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9be4a-107">Permissions</span></span>

<span data-ttu-id="9be4a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9be4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9be4a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9be4a-110">Permission type</span></span>                        | <span data-ttu-id="9be4a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9be4a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9be4a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9be4a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9be4a-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be4a-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9be4a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9be4a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be4a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be4a-115">Not supported.</span></span> |
| <span data-ttu-id="9be4a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9be4a-116">Application</span></span>                            | <span data-ttu-id="9be4a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be4a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9be4a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9be4a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9be4a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9be4a-119">Optional query parameters</span></span>

<span data-ttu-id="9be4a-120">Este método usa parâmetros de consulta OData para construir a resposta.</span><span class="sxs-lookup"><span data-stu-id="9be4a-120">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="9be4a-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9be4a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9be4a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9be4a-122">Request headers</span></span>

| <span data-ttu-id="9be4a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9be4a-123">Name</span></span>      |<span data-ttu-id="9be4a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9be4a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9be4a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9be4a-125">Authorization</span></span> | <span data-ttu-id="9be4a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9be4a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9be4a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9be4a-128">Request body</span></span>

<span data-ttu-id="9be4a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9be4a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9be4a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be4a-130">Response</span></span>

<span data-ttu-id="9be4a-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageResourceRole](../resources/accesspackageresourcerole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9be4a-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9be4a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9be4a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9be4a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9be4a-133">Request</span></span>

<span data-ttu-id="9be4a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9be4a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9be4a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9be4a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="9be4a-136">C#</span><span class="sxs-lookup"><span data-stu-id="9be4a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9be4a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9be4a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9be4a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9be4a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9be4a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be4a-139">Response</span></span>

<span data-ttu-id="9be4a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9be4a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="9be4a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9be4a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "displayName": "Member",
      "description": "description-value",
      "originId": "originId-value",
      "originSystem": "originSystem-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
