---
title: Criar site legalHoldSource
description: Criar um novo objeto legalHold siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: bca1f4c54593cc92f9b085bc86669981974e4432
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952449"
---
# <a name="create-legalhold-sitesource"></a><span data-ttu-id="4de8b-103">Criar site legalHoldSource</span><span class="sxs-lookup"><span data-stu-id="4de8b-103">Create legalHold siteSource</span></span>

<span data-ttu-id="4de8b-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4de8b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4de8b-105">Adiciona um siteSource a um objeto legalHold.</span><span class="sxs-lookup"><span data-stu-id="4de8b-105">Adds a siteSource to a legalHold object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4de8b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4de8b-106">Permissions</span></span>

<span data-ttu-id="4de8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4de8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4de8b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4de8b-109">Permission type</span></span>|<span data-ttu-id="4de8b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4de8b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4de8b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4de8b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4de8b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de8b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="4de8b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4de8b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4de8b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4de8b-114">Not supported.</span></span>|
|<span data-ttu-id="4de8b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4de8b-115">Application</span></span>|<span data-ttu-id="4de8b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4de8b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4de8b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4de8b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="4de8b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4de8b-118">Request headers</span></span>

|<span data-ttu-id="4de8b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4de8b-119">Name</span></span>|<span data-ttu-id="4de8b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4de8b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4de8b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4de8b-121">Authorization</span></span>|<span data-ttu-id="4de8b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4de8b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4de8b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4de8b-124">Content-Type</span></span>|<span data-ttu-id="4de8b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4de8b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4de8b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4de8b-127">Request body</span></span>

<span data-ttu-id="4de8b-128">No corpo da solicitação, fornece uma representação JSON do [objeto siteSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="4de8b-128">In the request body, supply a JSON representation of the [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

<span data-ttu-id="4de8b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o siteSource](../resources/ediscovery-sitesource.md).</span><span class="sxs-lookup"><span data-stu-id="4de8b-129">The following table shows the properties that are required when you create the [siteSource](../resources/ediscovery-sitesource.md).</span></span>

|<span data-ttu-id="4de8b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4de8b-130">Property</span></span>|<span data-ttu-id="4de8b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4de8b-131">Type</span></span>|<span data-ttu-id="4de8b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4de8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4de8b-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="4de8b-133">site@odata.bind</span></span>|<span data-ttu-id="4de8b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4de8b-134">String</span></span>|<span data-ttu-id="4de8b-135">ID do site, que você pode obter do recurso [de site](../resources/site.md) usando o método Obter um recurso de [site por](../api/site-getbypath.md) caminho.</span><span class="sxs-lookup"><span data-stu-id="4de8b-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="4de8b-136">O uso é {hostname}:/{relative-path}.</span><span class="sxs-lookup"><span data-stu-id="4de8b-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="4de8b-137">Para a URL do `https://contoso.sharepoint.com/sites/HumanResources` site, a solicitação do Microsoft Graph seria `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` .</span><span class="sxs-lookup"><span data-stu-id="4de8b-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="4de8b-138">A ID é o primeiro GUID listado no campo ID.</span><span class="sxs-lookup"><span data-stu-id="4de8b-138">The ID is the first GUID listed in the ID field.</span></span>  <span data-ttu-id="4de8b-139">Para a URL do site do OneDrive for `https://contoso-my.sharepoint.com/personal/adelev_contoso_com` business, a solicitação do Microsoft Graph seria `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`</span><span class="sxs-lookup"><span data-stu-id="4de8b-139">For the OneDrive for business site URL `https://contoso-my.sharepoint.com/personal/adelev_contoso_com`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`</span></span> |

## <a name="response"></a><span data-ttu-id="4de8b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4de8b-140">Response</span></span>

<span data-ttu-id="4de8b-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4de8b-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4de8b-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4de8b-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4de8b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4de8b-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4de8b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="4de8b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sitesource_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/siteSources
Content-Type: application/json
Content-length: 154

{
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181"
}
```
# <a name="c"></a>[<span data-ttu-id="4de8b-145">C#</span><span class="sxs-lookup"><span data-stu-id="4de8b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4de8b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4de8b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4de8b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4de8b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4de8b-148">Java</span><span class="sxs-lookup"><span data-stu-id="4de8b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4de8b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4de8b-149">Response</span></span>

<span data-ttu-id="4de8b-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4de8b-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.siteSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalHolds('387566cc-38ae-4e85-ab4b-cd2dd34faa07')/siteSources/$entity",
    "displayName": "Adele Vance",
    "createdDateTime": "2020-12-28T20:08:57.857Z",
    "id": "50073f3e-cb22-48e5-95a9-51a3da455181",
    "createdBy": {
        "user": {
            "id": null,
            "displayName": "EDiscovery admin"
        }
    }
}
```
