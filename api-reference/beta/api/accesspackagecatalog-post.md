---
title: Criar accessPackageCatalog
description: Criar um novo accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b973310b9cb442f2b95ba4eafd9a2e76ba33fce
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994208"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="ed507-103">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="ed507-103">Create accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed507-104">Criar um novo objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="ed507-104">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed507-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed507-105">Permissions</span></span>

<span data-ttu-id="ed507-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed507-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed507-108">Permission type</span></span>                        | <span data-ttu-id="ed507-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed507-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ed507-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed507-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed507-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed507-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ed507-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed507-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed507-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed507-113">Not supported.</span></span> |
| <span data-ttu-id="ed507-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed507-114">Application</span></span>                            | <span data-ttu-id="ed507-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed507-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed507-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed507-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="ed507-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed507-117">Request headers</span></span>

| <span data-ttu-id="ed507-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ed507-118">Name</span></span>          | <span data-ttu-id="ed507-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed507-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ed507-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed507-120">Authorization</span></span> | <span data-ttu-id="ed507-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="ed507-121">Bearer \{token\}.</span></span> <span data-ttu-id="ed507-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed507-122">Required.</span></span> |
| <span data-ttu-id="ed507-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed507-123">Content-Type</span></span>  | <span data-ttu-id="ed507-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ed507-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed507-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed507-125">Request body</span></span>

<span data-ttu-id="ed507-126">No corpo da solicitação, forneça uma representação JSON de um objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="ed507-126">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="ed507-127">Inclua as propriedades **DisplayName**, **Description**e **isExternallyVisible** .</span><span class="sxs-lookup"><span data-stu-id="ed507-127">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="ed507-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed507-128">Response</span></span>

<span data-ttu-id="ed507-129">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed507-129">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed507-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ed507-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed507-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed507-131">Request</span></span>

<span data-ttu-id="ed507-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed507-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ed507-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed507-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_accesspackagecatalogs"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
Content-type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "isExternallyVisible": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed507-134">C#</span><span class="sxs-lookup"><span data-stu-id="ed507-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed507-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed507-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed507-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed507-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed507-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed507-137">Response</span></span>

<span data-ttu-id="ed507-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed507-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ed507-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed507-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "UserManaged",
  "catalogStatus": "Published",
  "isExternallyVisible": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
