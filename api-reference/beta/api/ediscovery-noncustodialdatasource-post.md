---
title: Criar noncustodialDataSource
description: Crie um novo objeto noncustodialDataSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 840cddbdfa4c0172bdce85a46238e95d5f059a86
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52266656"
---
# <a name="create-noncustodialdatasource"></a><span data-ttu-id="dc6be-103">Criar noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="dc6be-103">Create noncustodialDataSource</span></span>

<span data-ttu-id="dc6be-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="dc6be-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc6be-105">Crie um novo [objeto noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="dc6be-105">Create a new [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc6be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc6be-106">Permissions</span></span>

<span data-ttu-id="dc6be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc6be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc6be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc6be-109">Permission type</span></span>|<span data-ttu-id="dc6be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc6be-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc6be-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc6be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc6be-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc6be-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="dc6be-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc6be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc6be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc6be-114">Not supported.</span></span>|
|<span data-ttu-id="dc6be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc6be-115">Application</span></span>|<span data-ttu-id="dc6be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc6be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc6be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc6be-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources
```

## <a name="request-headers"></a><span data-ttu-id="dc6be-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6be-118">Request headers</span></span>

|<span data-ttu-id="dc6be-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dc6be-119">Name</span></span>|<span data-ttu-id="dc6be-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc6be-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc6be-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc6be-121">Authorization</span></span>|<span data-ttu-id="dc6be-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc6be-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dc6be-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc6be-124">Content-Type</span></span>|<span data-ttu-id="dc6be-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc6be-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc6be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6be-127">Request body</span></span>

<span data-ttu-id="dc6be-128">No corpo da solicitação, fornece uma representação JSON do [objeto noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="dc6be-128">In the request body, supply a JSON representation of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

<span data-ttu-id="dc6be-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span><span class="sxs-lookup"><span data-stu-id="dc6be-129">The following table shows the properties that are required when you create the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).</span></span>

|<span data-ttu-id="dc6be-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc6be-130">Property</span></span>|<span data-ttu-id="dc6be-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc6be-131">Type</span></span>|<span data-ttu-id="dc6be-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc6be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc6be-133">applyHoldToSource</span><span class="sxs-lookup"><span data-stu-id="dc6be-133">applyHoldToSource</span></span>|<span data-ttu-id="dc6be-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="dc6be-134">Boolean</span></span>|<span data-ttu-id="dc6be-135">Indica se a espera é aplicada à fonte de dados não custodial (como caixa de correio ou site).</span><span class="sxs-lookup"><span data-stu-id="dc6be-135">Indicates if hold is applied to non-custodial data source (such as mailbox or site).</span></span>|
|<span data-ttu-id="dc6be-136">datasource</span><span class="sxs-lookup"><span data-stu-id="dc6be-136">datasource</span></span>|[<span data-ttu-id="dc6be-137">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="dc6be-137">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="dc6be-138">Um userSource ou siteSource.</span><span class="sxs-lookup"><span data-stu-id="dc6be-138">Either a userSource or siteSource.</span></span>  <span data-ttu-id="dc6be-139">Para userSource, use "dataSource" : { "@odata.type" : "microsoft.graph.ediscovery.userSource", "email" : "endereço SMTP"}.</span><span class="sxs-lookup"><span data-stu-id="dc6be-139">For userSource, use "dataSource" : { "@odata.type" : "microsoft.graph.ediscovery.userSource", "email" : "SMTP address"}.</span></span>  <span data-ttu-id="dc6be-140">Para a origem do site, use "dataSource" : { "@odata.type" : "microsoft.graph.ediscovery.siteSource", "site@odata.bind" : "siteId" }, onde siteId pode ser derivado da URL do site, por exemplo, a solicitação do `https://contoso.sharepoint.com/sites/HumanResources` Microsoft Graph seria `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` .</span><span class="sxs-lookup"><span data-stu-id="dc6be-140">For site source use "dataSource" : { "@odata.type" : "microsoft.graph.ediscovery.siteSource", "site@odata.bind" : "siteId" }, where siteId can be derived from the site URL, e.g. `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="dc6be-141">A ID é o primeiro GUID listado no campo ID.</span><span class="sxs-lookup"><span data-stu-id="dc6be-141">The ID is the first GUID listed in the ID field.</span></span>

## <a name="response"></a><span data-ttu-id="dc6be-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc6be-142">Response</span></span>

<span data-ttu-id="dc6be-143">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc6be-143">If successful, this method returns a `201 Created` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc6be-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dc6be-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc6be-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc6be-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dc6be-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc6be-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_noncustodialdatasource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources
Content-Type: application/json
Content-length: 206

{
    "applyHoldToSource" : true,
    "dataSource" : {
        "@odata.type" : "microsoft.graph.ediscovery.userSource",
        "email" : "adelev@contoso.com"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="dc6be-147">C#</span><span class="sxs-lookup"><span data-stu-id="dc6be-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-noncustodialdatasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc6be-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc6be-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-noncustodialdatasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc6be-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc6be-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-noncustodialdatasource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc6be-150">Java</span><span class="sxs-lookup"><span data-stu-id="dc6be-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-noncustodialdatasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc6be-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc6be-151">Response</span></span>

<span data-ttu-id="dc6be-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dc6be-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources/$entity",
    "status": "0",
    "lastModifiedDateTime": "2021-02-19T07:02:45.7732516Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "39374346363831303741353341373443",
    "displayName": null,
    "createdDateTime": "2021-02-19T07:02:45.4863718Z",
    "applyHoldToSource": true
}
```
