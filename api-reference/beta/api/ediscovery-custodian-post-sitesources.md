---
title: Criar site custodiadoSource
description: Criar um novo objeto custodiante siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 869f967073e4f41cf5d4cb40f18e9b7f6ba825d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773246"
---
# <a name="create-custodian-sitesource"></a><span data-ttu-id="b7158-103">Criar site custodiadoSource</span><span class="sxs-lookup"><span data-stu-id="b7158-103">Create custodian siteSource</span></span>

<span data-ttu-id="b7158-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b7158-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7158-105">Criar um novo objeto [custodiante siteSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="b7158-105">Create a new custodian [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7158-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b7158-106">Permissions</span></span>

<span data-ttu-id="b7158-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7158-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7158-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7158-109">Permission type</span></span>|<span data-ttu-id="b7158-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7158-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7158-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7158-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7158-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7158-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b7158-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7158-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7158-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7158-114">Not supported.</span></span>|
|<span data-ttu-id="b7158-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7158-115">Application</span></span>|<span data-ttu-id="b7158-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7158-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7158-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7158-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="b7158-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7158-118">Request headers</span></span>

|<span data-ttu-id="b7158-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b7158-119">Name</span></span>|<span data-ttu-id="b7158-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7158-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b7158-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7158-121">Authorization</span></span>|<span data-ttu-id="b7158-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7158-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b7158-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7158-124">Content-Type</span></span>|<span data-ttu-id="b7158-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7158-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7158-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7158-127">Request body</span></span>

<span data-ttu-id="b7158-128">No corpo da solicitação, fornece uma representação JSON do [objeto siteSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="b7158-128">In the request body, supply a JSON representation of the [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

<span data-ttu-id="b7158-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o siteSource](../resources/ediscovery-sitesource.md).</span><span class="sxs-lookup"><span data-stu-id="b7158-129">The following table shows the properties that are required when you create the [siteSource](../resources/ediscovery-sitesource.md).</span></span>

|<span data-ttu-id="b7158-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7158-130">Property</span></span>|<span data-ttu-id="b7158-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7158-131">Type</span></span>|<span data-ttu-id="b7158-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7158-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7158-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="b7158-133">site@odata.bind</span></span>|<span data-ttu-id="b7158-134">String</span><span class="sxs-lookup"><span data-stu-id="b7158-134">String</span></span>|<span data-ttu-id="b7158-135">ID do site, que você pode obter do recurso [de site](../resources/site.md) usando o método Obter um recurso de [site por](../api/site-getbypath.md) caminho.</span><span class="sxs-lookup"><span data-stu-id="b7158-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="b7158-136">O uso é {hostname}:/{relative-path}.</span><span class="sxs-lookup"><span data-stu-id="b7158-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="b7158-137">Para a URL do `https://contoso.sharepoint.com/sites/HumanResources` site, a solicitação do Microsoft Graph seria `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` .</span><span class="sxs-lookup"><span data-stu-id="b7158-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="b7158-138">A ID é o primeiro GUID listado no campo ID.</span><span class="sxs-lookup"><span data-stu-id="b7158-138">The ID is the first GUID listed in the ID field.</span></span>  <span data-ttu-id="b7158-139">Para a URL do site do OneDrive for `https://contoso-my.sharepoint.com/personal/adelev_contoso_com` Business, a solicitação do Microsoft Graph seria `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com` .</span><span class="sxs-lookup"><span data-stu-id="b7158-139">For the OneDrive for Business site URL `https://contoso-my.sharepoint.com/personal/adelev_contoso_com`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso-my.sharepoint.com:/personal/adelev_contoso_com`.</span></span> |

## <a name="response"></a><span data-ttu-id="b7158-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7158-140">Response</span></span>

<span data-ttu-id="b7158-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7158-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7158-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7158-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7158-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7158-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b7158-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7158-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sitesource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
Content-Type: application/json
Content-length: 179

{
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181"
}
```
# <a name="c"></a>[<span data-ttu-id="b7158-145">C#</span><span class="sxs-lookup"><span data-stu-id="b7158-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7158-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7158-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7158-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7158-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7158-148">Java</span><span class="sxs-lookup"><span data-stu-id="b7158-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7158-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7158-149">Response</span></span>

<span data-ttu-id="b7158-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b7158-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Human resources site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
