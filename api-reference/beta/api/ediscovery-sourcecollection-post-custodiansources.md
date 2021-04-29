---
title: Adicionar custodianSources
description: Adicionar objetos dataSource de custodia a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 4193bfa0f74461f284329cbb5772deee6417a029
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080278"
---
# <a name="add-custodiansources"></a><span data-ttu-id="255ce-103">Adicionar custodianSources</span><span class="sxs-lookup"><span data-stu-id="255ce-103">Add custodianSources</span></span>

<span data-ttu-id="255ce-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="255ce-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="255ce-105">Adicionar objetos [dataSource custodiantes](../resources/ediscovery-datasource.md) a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="255ce-105">Add custodian [dataSource](../resources/ediscovery-datasource.md) objects to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="255ce-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="255ce-106">Permissions</span></span>

<span data-ttu-id="255ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="255ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="255ce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="255ce-109">Permission type</span></span>|<span data-ttu-id="255ce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="255ce-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="255ce-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="255ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="255ce-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="255ce-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="255ce-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="255ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="255ce-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="255ce-114">Not supported.</span></span>|
|<span data-ttu-id="255ce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="255ce-115">Application</span></span>|<span data-ttu-id="255ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="255ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="255ce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="255ce-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="255ce-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="255ce-118">Request headers</span></span>

|<span data-ttu-id="255ce-119">Nome</span><span class="sxs-lookup"><span data-stu-id="255ce-119">Name</span></span>|<span data-ttu-id="255ce-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="255ce-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="255ce-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="255ce-121">Authorization</span></span>|<span data-ttu-id="255ce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="255ce-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="255ce-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="255ce-124">Content-Type</span></span>|<span data-ttu-id="255ce-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="255ce-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="255ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="255ce-127">Request body</span></span>

<span data-ttu-id="255ce-128">No corpo da solicitação, fornece uma representação JSON do [objeto dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="255ce-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="255ce-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o dataSource](../resources/ediscovery-datasource.md).</span><span class="sxs-lookup"><span data-stu-id="255ce-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="255ce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="255ce-130">Property</span></span>|<span data-ttu-id="255ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="255ce-131">Type</span></span>|<span data-ttu-id="255ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="255ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="255ce-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="255ce-133">@odata.id</span></span>|<span data-ttu-id="255ce-134">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="255ce-134">String</span></span>|<span data-ttu-id="255ce-135">Cadeia de caracteres que define o objeto custodial.</span><span class="sxs-lookup"><span data-stu-id="255ce-135">String that defines the custodial object.</span></span> <span data-ttu-id="255ce-136">Vejo o exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="255ce-136">See the example that follows.</span></span>|

## <a name="response"></a><span data-ttu-id="255ce-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="255ce-137">Response</span></span>

<span data-ttu-id="255ce-138">Se tiver êxito, este método retornará um código de resposta e um `204 No Content` [objeto microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="255ce-138">If successful, this method returns a `204 No Content` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="255ce-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="255ce-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="255ce-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="255ce-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="255ce-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="255ce-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_datasource_from__2"
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
# <a name="c"></a>[<span data-ttu-id="255ce-142">C#</span><span class="sxs-lookup"><span data-stu-id="255ce-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-datasource-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="255ce-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="255ce-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-datasource-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="255ce-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="255ce-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-datasource-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="255ce-145">Java</span><span class="sxs-lookup"><span data-stu-id="255ce-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-datasource-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="255ce-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="255ce-146">Response</span></span>

> <span data-ttu-id="255ce-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="255ce-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 204 No Content
```
