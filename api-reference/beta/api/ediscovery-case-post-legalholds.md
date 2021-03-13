---
title: Criar legalHold
description: Crie um novo objeto legalHold.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a48774cd3613b2b2cdbcb376d5ffe9781a786c79
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773848"
---
# <a name="create-legalhold"></a><span data-ttu-id="c2e78-103">Criar legalHold</span><span class="sxs-lookup"><span data-stu-id="c2e78-103">Create legalHold</span></span>

<span data-ttu-id="c2e78-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c2e78-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2e78-105">Crie um novo [objeto legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="c2e78-105">Create a new [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2e78-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2e78-106">Permissions</span></span>

<span data-ttu-id="c2e78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2e78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2e78-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2e78-109">Permission type</span></span>|<span data-ttu-id="c2e78-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2e78-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2e78-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2e78-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2e78-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2e78-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c2e78-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2e78-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2e78-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2e78-114">Not supported.</span></span>|
|<span data-ttu-id="c2e78-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2e78-115">Application</span></span>|<span data-ttu-id="c2e78-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2e78-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2e78-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2e78-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds
```

## <a name="request-headers"></a><span data-ttu-id="c2e78-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2e78-118">Request headers</span></span>

|<span data-ttu-id="c2e78-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c2e78-119">Name</span></span>|<span data-ttu-id="c2e78-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2e78-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c2e78-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2e78-121">Authorization</span></span>|<span data-ttu-id="c2e78-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2e78-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c2e78-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2e78-124">Content-Type</span></span>|<span data-ttu-id="c2e78-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2e78-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2e78-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2e78-127">Request body</span></span>

<span data-ttu-id="c2e78-128">No corpo da solicitação, fornece uma representação JSON do [objeto legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="c2e78-128">In the request body, supply a JSON representation of the [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

<span data-ttu-id="c2e78-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [legalHold](../resources/ediscovery-legalhold.md).</span><span class="sxs-lookup"><span data-stu-id="c2e78-129">The following table shows the properties that are required when you create the [legalHold](../resources/ediscovery-legalhold.md).</span></span>

|<span data-ttu-id="c2e78-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2e78-130">Property</span></span>|<span data-ttu-id="c2e78-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2e78-131">Type</span></span>|<span data-ttu-id="c2e78-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2e78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2e78-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c2e78-133">displayName</span></span>|<span data-ttu-id="c2e78-134">String</span><span class="sxs-lookup"><span data-stu-id="c2e78-134">String</span></span>| <span data-ttu-id="c2e78-135">O nome de exibição da ressução legal.</span><span class="sxs-lookup"><span data-stu-id="c2e78-135">The display name of the legal hold.</span></span> |

## <a name="response"></a><span data-ttu-id="c2e78-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2e78-136">Response</span></span>

<span data-ttu-id="c2e78-137">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2e78-137">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2e78-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c2e78-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2e78-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2e78-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c2e78-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2e78-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_legalhold_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds
Content-Type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="c2e78-141">C#</span><span class="sxs-lookup"><span data-stu-id="c2e78-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-legalhold-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2e78-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2e78-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-legalhold-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2e78-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2e78-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-legalhold-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2e78-144">Java</span><span class="sxs-lookup"><span data-stu-id="c2e78-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-legalhold-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2e78-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2e78-145">Response</span></span>

<span data-ttu-id="c2e78-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c2e78-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "id": "700cd868-d868-700c-68d8-0c7068d80c70",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
