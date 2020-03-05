---
title: Criar accessPackageCatalog
description: Criar um novo accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90a340de45fc0f31e1b5bd534151c449a2b315af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441960"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="dfb76-103">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="dfb76-103">Create accessPackageCatalog</span></span>

<span data-ttu-id="dfb76-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dfb76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfb76-105">Criar um novo objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="dfb76-105">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfb76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfb76-106">Permissions</span></span>

<span data-ttu-id="dfb76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfb76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfb76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfb76-109">Permission type</span></span>                        | <span data-ttu-id="dfb76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfb76-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dfb76-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfb76-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfb76-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfb76-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="dfb76-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfb76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfb76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfb76-114">Not supported.</span></span> |
| <span data-ttu-id="dfb76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfb76-115">Application</span></span>                            | <span data-ttu-id="dfb76-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfb76-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfb76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfb76-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="dfb76-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb76-118">Request headers</span></span>

| <span data-ttu-id="dfb76-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dfb76-119">Name</span></span>          | <span data-ttu-id="dfb76-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfb76-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dfb76-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfb76-121">Authorization</span></span> | <span data-ttu-id="dfb76-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="dfb76-122">Bearer \{token\}.</span></span> <span data-ttu-id="dfb76-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfb76-123">Required.</span></span> |
| <span data-ttu-id="dfb76-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfb76-124">Content-Type</span></span>  | <span data-ttu-id="dfb76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfb76-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfb76-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb76-126">Request body</span></span>

<span data-ttu-id="dfb76-127">No corpo da solicitação, forneça uma representação JSON de um objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="dfb76-127">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="dfb76-128">Inclua as propriedades **DisplayName**, **Description**e **isExternallyVisible** .</span><span class="sxs-lookup"><span data-stu-id="dfb76-128">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="dfb76-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb76-129">Response</span></span>

<span data-ttu-id="dfb76-130">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfb76-130">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfb76-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dfb76-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dfb76-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb76-132">Request</span></span>

<span data-ttu-id="dfb76-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfb76-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfb76-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfb76-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dfb76-135">C#</span><span class="sxs-lookup"><span data-stu-id="dfb76-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfb76-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfb76-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfb76-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfb76-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dfb76-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb76-138">Response</span></span>

<span data-ttu-id="dfb76-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfb76-139">The following is an example of the response.</span></span>

> <span data-ttu-id="dfb76-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfb76-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
