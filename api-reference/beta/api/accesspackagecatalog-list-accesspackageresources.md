---
title: Listar accessPackageResources
description: Recupere uma lista de objetos accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1b516920f1f1c75587348738598d2a540ceac23b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994264"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="7c8b9-103">Listar accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="7c8b9-103">List accessPackageResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c8b9-104">Recupere uma lista de objetos [accessPackageResource](../resources/accesspackageresource.md) em um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="7c8b9-104">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c8b9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c8b9-105">Permissions</span></span>

<span data-ttu-id="7c8b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c8b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c8b9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c8b9-108">Permission type</span></span>                        | <span data-ttu-id="7c8b9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c8b9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7c8b9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c8b9-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="7c8b9-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c8b9-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7c8b9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c8b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c8b9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-113">Not supported.</span></span> |
| <span data-ttu-id="7c8b9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c8b9-114">Application</span></span>                            | <span data-ttu-id="7c8b9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c8b9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c8b9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c8b9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c8b9-117">Optional query parameters</span></span>

<span data-ttu-id="7c8b9-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7c8b9-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7c8b9-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c8b9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8b9-120">Request headers</span></span>

| <span data-ttu-id="7c8b9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7c8b9-121">Name</span></span>      |<span data-ttu-id="7c8b9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c8b9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7c8b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c8b9-123">Authorization</span></span> | <span data-ttu-id="7c8b9-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-124">Bearer \{token\}.</span></span> <span data-ttu-id="7c8b9-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c8b9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8b9-126">Request body</span></span>

<span data-ttu-id="7c8b9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c8b9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8b9-128">Response</span></span>

<span data-ttu-id="7c8b9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageResource](../resources/accesspackageresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-129">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c8b9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7c8b9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c8b9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8b9-131">Request</span></span>

<span data-ttu-id="7c8b9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7c8b9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c8b9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7c8b9-134">C#</span><span class="sxs-lookup"><span data-stu-id="7c8b9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c8b9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c8b9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c8b9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c8b9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7c8b9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8b9-137">Response</span></span>

<span data-ttu-id="7c8b9-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-138">The following is an example of the response.</span></span>

> <span data-ttu-id="7c8b9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c8b9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
