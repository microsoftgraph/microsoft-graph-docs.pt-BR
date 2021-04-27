---
title: Criar accessPackageCatalog
description: Crie um novo accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a9a1190c09cff042783284205def04de3ec4e700
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048544"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="004cb-103">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="004cb-103">Create accessPackageCatalog</span></span>

<span data-ttu-id="004cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="004cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="004cb-105">Crie um novo [objeto accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="004cb-105">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="004cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="004cb-106">Permissions</span></span>

<span data-ttu-id="004cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="004cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="004cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="004cb-109">Permission type</span></span>                        | <span data-ttu-id="004cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="004cb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="004cb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="004cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="004cb-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004cb-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="004cb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="004cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="004cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="004cb-114">Not supported.</span></span> |
| <span data-ttu-id="004cb-115">Application</span><span class="sxs-lookup"><span data-stu-id="004cb-115">Application</span></span>                            | <span data-ttu-id="004cb-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004cb-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="004cb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="004cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="004cb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="004cb-118">Request headers</span></span>

| <span data-ttu-id="004cb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="004cb-119">Name</span></span>          | <span data-ttu-id="004cb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="004cb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="004cb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="004cb-121">Authorization</span></span> | <span data-ttu-id="004cb-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="004cb-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="004cb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="004cb-124">Content-Type</span></span>  | <span data-ttu-id="004cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="004cb-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="004cb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="004cb-126">Request body</span></span>

<span data-ttu-id="004cb-127">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="004cb-127">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="004cb-128">Inclua as **propriedades displayname**, **description** e **isExternallyVisible.**</span><span class="sxs-lookup"><span data-stu-id="004cb-128">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="004cb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="004cb-129">Response</span></span>

<span data-ttu-id="004cb-130">Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="004cb-130">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="004cb-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="004cb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="004cb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="004cb-132">Request</span></span>

<span data-ttu-id="004cb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="004cb-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="004cb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="004cb-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="004cb-135">C#</span><span class="sxs-lookup"><span data-stu-id="004cb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="004cb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="004cb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="004cb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="004cb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="004cb-138">Java</span><span class="sxs-lookup"><span data-stu-id="004cb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackagecatalog-from-accesspackagecatalogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="004cb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="004cb-139">Response</span></span>

<span data-ttu-id="004cb-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="004cb-140">The following is an example of the response.</span></span>

> <span data-ttu-id="004cb-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="004cb-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


