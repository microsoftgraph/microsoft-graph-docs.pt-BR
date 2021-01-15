---
title: Criar siteSource
description: Criar um novo objeto siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 8502084d1b4519c74042788e02fdf3636540535e
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872559"
---
# <a name="create-sitesource"></a><span data-ttu-id="efeb5-103">Criar siteSource</span><span class="sxs-lookup"><span data-stu-id="efeb5-103">Create siteSource</span></span>

<span data-ttu-id="efeb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efeb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efeb5-105">Criar um novo [objeto siteSource.](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="efeb5-105">Create a new [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="efeb5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="efeb5-106">Permissions</span></span>

<span data-ttu-id="efeb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efeb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efeb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efeb5-109">Permission type</span></span>|<span data-ttu-id="efeb5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efeb5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efeb5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efeb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="efeb5-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="efeb5-112">User.Read</span></span>|
|<span data-ttu-id="efeb5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efeb5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efeb5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efeb5-114">Not supported.</span></span>|
|<span data-ttu-id="efeb5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efeb5-115">Application</span></span>|<span data-ttu-id="efeb5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efeb5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efeb5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efeb5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="efeb5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efeb5-118">Request headers</span></span>

|<span data-ttu-id="efeb5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="efeb5-119">Name</span></span>|<span data-ttu-id="efeb5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="efeb5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="efeb5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="efeb5-121">Authorization</span></span>|<span data-ttu-id="efeb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efeb5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="efeb5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="efeb5-124">Content-Type</span></span>|<span data-ttu-id="efeb5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efeb5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="efeb5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efeb5-127">Request body</span></span>

<span data-ttu-id="efeb5-128">No corpo da solicitação, fornece uma representação JSON do [objeto siteSource.](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="efeb5-128">In the request body, supply a JSON representation of the [siteSource](../resources/sitesource.md) object.</span></span>

<span data-ttu-id="efeb5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [siteSource](../resources/sitesource.md).</span><span class="sxs-lookup"><span data-stu-id="efeb5-129">The following table shows the properties that are required when you create the [siteSource](../resources/sitesource.md).</span></span>

|<span data-ttu-id="efeb5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efeb5-130">Property</span></span>|<span data-ttu-id="efeb5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efeb5-131">Type</span></span>|<span data-ttu-id="efeb5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efeb5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efeb5-133">site@odata.bind</span><span class="sxs-lookup"><span data-stu-id="efeb5-133">site@odata.bind</span></span>|<span data-ttu-id="efeb5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efeb5-134">String</span></span>|<span data-ttu-id="efeb5-135">ID do site, que você pode obter do recurso [de site](../resources/site.md) usando o método Obter um recurso de [site por](../api/site-getbypath.md) caminho.</span><span class="sxs-lookup"><span data-stu-id="efeb5-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="efeb5-136">O uso é {hostname}:/{relative-path}.</span><span class="sxs-lookup"><span data-stu-id="efeb5-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="efeb5-137">Para a URL do `https://contoso.sharepoint.com/sites/HumanResources` site, a solicitação do Microsoft Graph `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` seria.</span><span class="sxs-lookup"><span data-stu-id="efeb5-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="efeb5-138">A ID é o primeiro GUID listado no campo de ID.</span><span class="sxs-lookup"><span data-stu-id="efeb5-138">The ID is the first GUID listed in the ID field.</span></span>|

## <a name="response"></a><span data-ttu-id="efeb5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="efeb5-139">Response</span></span>

<span data-ttu-id="efeb5-140">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto siteSource](../resources/sitesource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efeb5-140">If successful, this method returns a `201 Created` response code and a [siteSource](../resources/sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efeb5-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="efeb5-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efeb5-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efeb5-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="efeb5-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="efeb5-143">HTTP</span></span>](#tab/http)
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
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/{siteId}"
}
```
# <a name="c"></a>[<span data-ttu-id="efeb5-144">C#</span><span class="sxs-lookup"><span data-stu-id="efeb5-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efeb5-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efeb5-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efeb5-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efeb5-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efeb5-147">Java</span><span class="sxs-lookup"><span data-stu-id="efeb5-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="efeb5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="efeb5-148">Response</span></span>

<span data-ttu-id="efeb5-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="efeb5-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteSource"
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
