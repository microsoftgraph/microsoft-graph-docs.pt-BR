---
title: Atualizar accessPackage
description: Atualize as propriedades de um objeto accessPackage.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 40f299edcca636a6f2041a36e10b0dc3963d8422
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439762"
---
# <a name="update-accesspackage"></a><span data-ttu-id="da3e4-103">Atualizar accessPackage</span><span class="sxs-lookup"><span data-stu-id="da3e4-103">Update accessPackage</span></span>

<span data-ttu-id="da3e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da3e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da3e4-105">Atualize um objeto [accessPackage](../resources/accesspackage.md) existente para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.</span><span class="sxs-lookup"><span data-stu-id="da3e4-105">Update an existing [accessPackage](../resources/accesspackage.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="da3e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="da3e4-106">Permissions</span></span>
<span data-ttu-id="da3e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="da3e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="da3e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da3e4-109">Permission type</span></span>|<span data-ttu-id="da3e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da3e4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da3e4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da3e4-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3e4-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="da3e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da3e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da3e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da3e4-114">Not supported.</span></span> |
|<span data-ttu-id="da3e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da3e4-115">Application</span></span>                            | <span data-ttu-id="da3e4-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3e4-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da3e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da3e4-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```
## <a name="request-headers"></a><span data-ttu-id="da3e4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da3e4-118">Request headers</span></span>
|<span data-ttu-id="da3e4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="da3e4-119">Name</span></span>|<span data-ttu-id="da3e4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="da3e4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da3e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="da3e4-121">Authorization</span></span>|<span data-ttu-id="da3e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da3e4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="da3e4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da3e4-124">Content-Type</span></span>|<span data-ttu-id="da3e4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da3e4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da3e4-127">Request body</span></span>
<span data-ttu-id="da3e4-128">No corpo da solicitação, fornece uma representação JSON dos parâmetros de um [objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="da3e4-128">In the request body, supply a JSON representation of the parameters of an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="da3e4-129">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza [um accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="da3e4-129">The following table shows the properties that can be supplied when you update an [accessPackage](../resources/accesspackage.md).</span></span>

|<span data-ttu-id="da3e4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da3e4-130">Property</span></span>|<span data-ttu-id="da3e4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="da3e4-131">Type</span></span>|<span data-ttu-id="da3e4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="da3e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da3e4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="da3e4-133">displayName</span></span>|<span data-ttu-id="da3e4-134">String</span><span class="sxs-lookup"><span data-stu-id="da3e4-134">String</span></span>|<span data-ttu-id="da3e4-135">O nome do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="da3e4-135">The access package name.</span></span>|
|<span data-ttu-id="da3e4-136">descrição</span><span class="sxs-lookup"><span data-stu-id="da3e4-136">description</span></span>|<span data-ttu-id="da3e4-137">String</span><span class="sxs-lookup"><span data-stu-id="da3e4-137">String</span></span>|<span data-ttu-id="da3e4-138">A descrição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="da3e4-138">The description of the access package.</span></span>|

## <a name="response"></a><span data-ttu-id="da3e4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="da3e4-139">Response</span></span>
<span data-ttu-id="da3e4-140">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="da3e4-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="da3e4-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da3e4-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da3e4-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da3e4-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="da3e4-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="da3e4-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
Content-Type: application/json
Content-length: 38

{
  "displayName":"Access Package New Name"
}
```
# <a name="c"></a>[<span data-ttu-id="da3e4-144">C#</span><span class="sxs-lookup"><span data-stu-id="da3e4-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da3e4-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da3e4-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da3e4-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da3e4-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da3e4-147">Java</span><span class="sxs-lookup"><span data-stu-id="da3e4-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="da3e4-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="da3e4-148">Response</span></span>

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
  "description": "Update accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


