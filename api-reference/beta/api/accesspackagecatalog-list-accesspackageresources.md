---
title: Listar accessPackageResources
description: Recupere uma lista de objetos accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 726fdf04818717167b9909f02b43f3e333636e28
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441974"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="e25bc-103">Listar accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="e25bc-103">List accessPackageResources</span></span>

<span data-ttu-id="e25bc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e25bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e25bc-105">Recupere uma lista de objetos [accessPackageResource](../resources/accesspackageresource.md) em um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="e25bc-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e25bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e25bc-106">Permissions</span></span>

<span data-ttu-id="e25bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e25bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e25bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e25bc-109">Permission type</span></span>                        | <span data-ttu-id="e25bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e25bc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e25bc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e25bc-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="e25bc-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e25bc-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="e25bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e25bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e25bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e25bc-114">Not supported.</span></span> |
| <span data-ttu-id="e25bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e25bc-115">Application</span></span>                            | <span data-ttu-id="e25bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e25bc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e25bc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e25bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e25bc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e25bc-118">Optional query parameters</span></span>

<span data-ttu-id="e25bc-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e25bc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e25bc-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e25bc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e25bc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e25bc-121">Request headers</span></span>

| <span data-ttu-id="e25bc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e25bc-122">Name</span></span>      |<span data-ttu-id="e25bc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e25bc-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e25bc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e25bc-124">Authorization</span></span> | <span data-ttu-id="e25bc-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="e25bc-125">Bearer \{token\}.</span></span> <span data-ttu-id="e25bc-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e25bc-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e25bc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e25bc-127">Request body</span></span>

<span data-ttu-id="e25bc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e25bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e25bc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e25bc-129">Response</span></span>

<span data-ttu-id="e25bc-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageResource](../resources/accesspackageresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e25bc-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e25bc-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e25bc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e25bc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e25bc-132">Request</span></span>

<span data-ttu-id="e25bc-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e25bc-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e25bc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e25bc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="e25bc-135">C#</span><span class="sxs-lookup"><span data-stu-id="e25bc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e25bc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e25bc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e25bc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e25bc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e25bc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e25bc-138">Response</span></span>

<span data-ttu-id="e25bc-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e25bc-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e25bc-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e25bc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
