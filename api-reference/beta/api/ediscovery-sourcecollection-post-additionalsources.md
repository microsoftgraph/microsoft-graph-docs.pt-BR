---
title: Criar dataSource
description: Adicione fontes de dados adicionais a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 61da920c39cb75583661fde46c9bdbcc0a5d568d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772594"
---
# <a name="create-datasource"></a><span data-ttu-id="e25f0-103">Criar dataSource</span><span class="sxs-lookup"><span data-stu-id="e25f0-103">Create dataSource</span></span>

<span data-ttu-id="e25f0-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e25f0-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e25f0-105">Adicione fontes de dados adicionais a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="e25f0-105">Add additional data sources to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="e25f0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e25f0-106">Permissions</span></span>

<span data-ttu-id="e25f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e25f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e25f0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e25f0-109">Permission type</span></span>|<span data-ttu-id="e25f0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e25f0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e25f0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e25f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e25f0-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e25f0-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e25f0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e25f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e25f0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e25f0-114">Not supported.</span></span>|
|<span data-ttu-id="e25f0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e25f0-115">Application</span></span>|<span data-ttu-id="e25f0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e25f0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e25f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e25f0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="request-headers"></a><span data-ttu-id="e25f0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e25f0-118">Request headers</span></span>

|<span data-ttu-id="e25f0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e25f0-119">Name</span></span>|<span data-ttu-id="e25f0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e25f0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e25f0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e25f0-121">Authorization</span></span>|<span data-ttu-id="e25f0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e25f0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e25f0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e25f0-124">Content-Type</span></span>|<span data-ttu-id="e25f0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e25f0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e25f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e25f0-127">Request body</span></span>

<span data-ttu-id="e25f0-128">No corpo da solicitação, fornece uma representação JSON do [objeto dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="e25f0-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="e25f0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o dataSource](../resources/ediscovery-datasource.md).</span><span class="sxs-lookup"><span data-stu-id="e25f0-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="e25f0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e25f0-130">Property</span></span>|<span data-ttu-id="e25f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e25f0-131">Type</span></span>|<span data-ttu-id="e25f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e25f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e25f0-133">id</span><span class="sxs-lookup"><span data-stu-id="e25f0-133">id</span></span>|<span data-ttu-id="e25f0-134">String</span><span class="sxs-lookup"><span data-stu-id="e25f0-134">String</span></span>|<span data-ttu-id="e25f0-135">A ID do [caso sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="e25f0-135">The ID for [sourceCollection](../resources/ediscovery-sourcecollection.md) case.</span></span> <span data-ttu-id="e25f0-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e25f0-136">Read-only.</span></span> <span data-ttu-id="e25f0-137">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="e25f0-137">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="e25f0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e25f0-138">displayName</span></span>|<span data-ttu-id="e25f0-139">String</span><span class="sxs-lookup"><span data-stu-id="e25f0-139">String</span></span>|<span data-ttu-id="e25f0-140">O nome da [sourceCollection](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="e25f0-140">The name of the [sourceCollection](../resources/ediscovery-sourcecollection.md)</span></span>|
|<span data-ttu-id="e25f0-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e25f0-141">createdDateTime</span></span>|<span data-ttu-id="e25f0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e25f0-142">DateTimeOffset</span></span>|<span data-ttu-id="e25f0-143">A data e a hora em [que o sourceCollection](../resources/ediscovery-sourcecollection.md) foi criado.</span><span class="sxs-lookup"><span data-stu-id="e25f0-143">The date and time when the [sourceCollection](../resources/ediscovery-sourcecollection.md) was created.</span></span>|
|<span data-ttu-id="e25f0-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="e25f0-144">createdBy</span></span>|[<span data-ttu-id="e25f0-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="e25f0-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="e25f0-146">O usuário que criou [o sourceCollection](../resources/ediscovery-sourcecollection.md).</span><span class="sxs-lookup"><span data-stu-id="e25f0-146">The user who created the [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>|

## <a name="response"></a><span data-ttu-id="e25f0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e25f0-147">Response</span></span>

<span data-ttu-id="e25f0-148">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e25f0-148">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e25f0-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e25f0-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e25f0-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e25f0-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e25f0-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e25f0-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
Content-Type: application/json
Content-length: 179

{
    "@odata.type": "#microsoft.graph.ediscovery.userSource",
    "email": "badguy@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="e25f0-152">C#</span><span class="sxs-lookup"><span data-stu-id="e25f0-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-datasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e25f0-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e25f0-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-datasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e25f0-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e25f0-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-datasource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e25f0-155">Java</span><span class="sxs-lookup"><span data-stu-id="e25f0-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-datasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e25f0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="e25f0-156">Response</span></span>

<span data-ttu-id="e25f0-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e25f0-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "id": "0fb67fc5-7fc5-0fb6-c57f-b60fc57fb60f",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```
