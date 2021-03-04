---
title: Atualizar accessPackageCatalog
description: Atualize as propriedades de um objeto accessPackageCatalog.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: de8173002582bc55aa3e59b7fbaa966240e0076e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439482"
---
# <a name="update-accesspackagecatalog"></a><span data-ttu-id="8dc6c-103">Atualizar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="8dc6c-103">Update accessPackageCatalog</span></span>

<span data-ttu-id="8dc6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dc6c-105">Atualize um objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) existente para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.</span><span class="sxs-lookup"><span data-stu-id="8dc6c-105">Update an existing [accessPackageCatalog](../resources/accesspackagecatalog.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dc6c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8dc6c-106">Permissions</span></span>
<span data-ttu-id="8dc6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8dc6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="8dc6c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dc6c-109">Permission type</span></span>|<span data-ttu-id="8dc6c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8dc6c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dc6c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dc6c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dc6c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc6c-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="8dc6c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dc6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dc6c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dc6c-114">Not supported.</span></span> |
|<span data-ttu-id="8dc6c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dc6c-115">Application</span></span>                            | <span data-ttu-id="8dc6c-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc6c-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dc6c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dc6c-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a><span data-ttu-id="8dc6c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc6c-118">Request headers</span></span>
|<span data-ttu-id="8dc6c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8dc6c-119">Name</span></span>|<span data-ttu-id="8dc6c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc6c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8dc6c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8dc6c-121">Authorization</span></span>|<span data-ttu-id="8dc6c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dc6c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8dc6c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dc6c-124">Content-Type</span></span>|<span data-ttu-id="8dc6c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dc6c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dc6c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc6c-127">Request body</span></span>
<span data-ttu-id="8dc6c-128">No corpo da solicitação, fornece uma representação JSON do [objeto accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="8dc6c-128">In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

<span data-ttu-id="8dc6c-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="8dc6c-129">The following table shows the properties that are required when you update the [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

|<span data-ttu-id="8dc6c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dc6c-130">Property</span></span>|<span data-ttu-id="8dc6c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dc6c-131">Type</span></span>|<span data-ttu-id="8dc6c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dc6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc6c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8dc6c-133">displayName</span></span>|<span data-ttu-id="8dc6c-134">String</span><span class="sxs-lookup"><span data-stu-id="8dc6c-134">String</span></span>|<span data-ttu-id="8dc6c-135">O nome do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="8dc6c-135">The access package catalog name.</span></span>|
|<span data-ttu-id="8dc6c-136">descrição</span><span class="sxs-lookup"><span data-stu-id="8dc6c-136">description</span></span>|<span data-ttu-id="8dc6c-137">String</span><span class="sxs-lookup"><span data-stu-id="8dc6c-137">String</span></span>|<span data-ttu-id="8dc6c-138">A descrição do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="8dc6c-138">The description of the access package catalog.</span></span>|

## <a name="response"></a><span data-ttu-id="8dc6c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dc6c-139">Response</span></span>
<span data-ttu-id="8dc6c-140">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8dc6c-140">If successful, this method returns a `204 No Content` response code.</span></span>



## <a name="examples"></a><span data-ttu-id="8dc6c-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8dc6c-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8dc6c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dc6c-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8dc6c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dc6c-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8dc6c-144">C#</span><span class="sxs-lookup"><span data-stu-id="8dc6c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8dc6c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dc6c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8dc6c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dc6c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8dc6c-147">Java</span><span class="sxs-lookup"><span data-stu-id="8dc6c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8dc6c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dc6c-148">Response</span></span>

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


