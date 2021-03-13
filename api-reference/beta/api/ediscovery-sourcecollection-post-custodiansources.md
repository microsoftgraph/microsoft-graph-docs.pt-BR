---
title: Adicionar custodianSources
description: Adicionar objetos dataSource de custodia a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: aa5f895046548e43b982511be36587e989c38b67
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772573"
---
# <a name="add-custodiansources"></a><span data-ttu-id="69436-103">Adicionar custodianSources</span><span class="sxs-lookup"><span data-stu-id="69436-103">Add custodianSources</span></span>

<span data-ttu-id="69436-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="69436-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69436-105">Adicionar objetos [dataSource custodiantes](../resources/ediscovery-datasource.md) a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="69436-105">Add custodian [dataSource](../resources/ediscovery-datasource.md) objects to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="69436-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="69436-106">Permissions</span></span>

<span data-ttu-id="69436-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69436-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69436-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69436-109">Permission type</span></span>|<span data-ttu-id="69436-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69436-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69436-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69436-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69436-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69436-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="69436-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69436-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69436-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69436-114">Not supported.</span></span>|
|<span data-ttu-id="69436-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69436-115">Application</span></span>|<span data-ttu-id="69436-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69436-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69436-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69436-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="69436-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69436-118">Request headers</span></span>

|<span data-ttu-id="69436-119">Nome</span><span class="sxs-lookup"><span data-stu-id="69436-119">Name</span></span>|<span data-ttu-id="69436-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="69436-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69436-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="69436-121">Authorization</span></span>|<span data-ttu-id="69436-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69436-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="69436-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69436-124">Content-Type</span></span>|<span data-ttu-id="69436-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69436-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69436-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69436-127">Request body</span></span>

<span data-ttu-id="69436-128">No corpo da solicitação, fornece uma representação JSON do [objeto dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="69436-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="69436-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o dataSource](../resources/ediscovery-datasource.md).</span><span class="sxs-lookup"><span data-stu-id="69436-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="69436-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69436-130">Property</span></span>|<span data-ttu-id="69436-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="69436-131">Type</span></span>|<span data-ttu-id="69436-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="69436-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69436-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="69436-133">@odata.id</span></span>|<span data-ttu-id="69436-134">String</span><span class="sxs-lookup"><span data-stu-id="69436-134">String</span></span>|<span data-ttu-id="69436-135">Cadeia de caracteres que define o objeto custodial.</span><span class="sxs-lookup"><span data-stu-id="69436-135">String that defines the custodial object.</span></span> <span data-ttu-id="69436-136">Vejo o exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="69436-136">See the example that follows.</span></span>|

## <a name="response"></a><span data-ttu-id="69436-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="69436-137">Response</span></span>

<span data-ttu-id="69436-138">Se tiver êxito, este método retornará um código de resposta e um `204 No Content` [objeto microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69436-138">If successful, this method returns a `204 No Content` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69436-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="69436-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69436-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69436-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="69436-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="69436-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/custodianSources/$ref
Content-Type: application/json
Content-length: 179

{
  "@odata.id":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"
}
```
# <a name="c"></a>[<span data-ttu-id="69436-142">C#</span><span class="sxs-lookup"><span data-stu-id="69436-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-datasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69436-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69436-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-datasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69436-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69436-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-datasource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69436-145">Java</span><span class="sxs-lookup"><span data-stu-id="69436-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-datasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="69436-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="69436-146">Response</span></span>

<span data-ttu-id="69436-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="69436-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 204 No Content
Content-Type: application/json
```
