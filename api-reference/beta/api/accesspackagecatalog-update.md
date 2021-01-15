---
title: Atualizar accessPackageCatalog
description: Atualizar as propriedades de um objeto accessPackageCatalog.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c7bb4b1cadfd3991f19ff02b5ad596f5a8ff1491
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872160"
---
# <a name="update-accesspackagecatalog"></a><span data-ttu-id="e15f2-103">Atualizar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="e15f2-103">Update accessPackageCatalog</span></span>

<span data-ttu-id="e15f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e15f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e15f2-105">Atualize um objeto [accessPackageCatalog existente](../resources/accesspackagecatalog.md) para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.</span><span class="sxs-lookup"><span data-stu-id="e15f2-105">Update an existing [accessPackageCatalog](../resources/accesspackagecatalog.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="e15f2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e15f2-106">Permissions</span></span>
<span data-ttu-id="e15f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e15f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="e15f2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e15f2-109">Permission type</span></span>|<span data-ttu-id="e15f2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e15f2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e15f2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e15f2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e15f2-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15f2-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="e15f2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e15f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e15f2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e15f2-114">Not supported.</span></span> |
|<span data-ttu-id="e15f2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e15f2-115">Application</span></span>                            | <span data-ttu-id="e15f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e15f2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e15f2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e15f2-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a><span data-ttu-id="e15f2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e15f2-118">Request headers</span></span>
|<span data-ttu-id="e15f2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e15f2-119">Name</span></span>|<span data-ttu-id="e15f2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e15f2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e15f2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e15f2-121">Authorization</span></span>|<span data-ttu-id="e15f2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e15f2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e15f2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e15f2-124">Content-Type</span></span>|<span data-ttu-id="e15f2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e15f2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e15f2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e15f2-127">Request body</span></span>
<span data-ttu-id="e15f2-128">No corpo da solicitação, fornece uma representação JSON do [objeto accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="e15f2-128">In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

<span data-ttu-id="e15f2-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="e15f2-129">The following table shows the properties that are required when you update the [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

|<span data-ttu-id="e15f2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e15f2-130">Property</span></span>|<span data-ttu-id="e15f2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e15f2-131">Type</span></span>|<span data-ttu-id="e15f2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e15f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e15f2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e15f2-133">displayName</span></span>|<span data-ttu-id="e15f2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f2-134">String</span></span>|<span data-ttu-id="e15f2-135">O nome do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="e15f2-135">The access package catalog name.</span></span>|
|<span data-ttu-id="e15f2-136">description</span><span class="sxs-lookup"><span data-stu-id="e15f2-136">description</span></span>|<span data-ttu-id="e15f2-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f2-137">String</span></span>|<span data-ttu-id="e15f2-138">A descrição do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="e15f2-138">The description of the access package catalog.</span></span>|

## <a name="response"></a><span data-ttu-id="e15f2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e15f2-139">Response</span></span>
<span data-ttu-id="e15f2-140">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e15f2-140">If successful, this method returns a `204 No Content` response code.</span></span>



## <a name="examples"></a><span data-ttu-id="e15f2-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e15f2-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e15f2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e15f2-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e15f2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e15f2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
Content-Type: application/json
Content-length: 39

{
  "displayName":"Catalog One"
}
```
# <a name="c"></a>[<span data-ttu-id="e15f2-144">C#</span><span class="sxs-lookup"><span data-stu-id="e15f2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e15f2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e15f2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e15f2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e15f2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e15f2-147">Java</span><span class="sxs-lookup"><span data-stu-id="e15f2-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e15f2-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e15f2-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


