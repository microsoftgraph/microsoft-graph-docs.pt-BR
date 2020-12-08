---
title: Criar site local
description: Criar um novo objeto sitery.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 93cb37a6ff94a52830675f876084fc85a6365a40
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597489"
---
# <a name="create-sitesource"></a><span data-ttu-id="4e953-103">Criar site local</span><span class="sxs-lookup"><span data-stu-id="4e953-103">Create siteSource</span></span>

<span data-ttu-id="4e953-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4e953-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e953-105">Criar um novo objeto [sitery](../resources/sitesource.md) .</span><span class="sxs-lookup"><span data-stu-id="4e953-105">Create a new [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e953-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4e953-106">Permissions</span></span>

<span data-ttu-id="4e953-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e953-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e953-109">Permission type</span></span>|<span data-ttu-id="4e953-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e953-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e953-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e953-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4e953-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="4e953-112">User.Read</span></span>|
|<span data-ttu-id="4e953-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e953-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e953-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e953-114">Not supported.</span></span>|
|<span data-ttu-id="4e953-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e953-115">Application</span></span>|<span data-ttu-id="4e953-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e953-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e953-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e953-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a><span data-ttu-id="4e953-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e953-118">Request headers</span></span>

|<span data-ttu-id="4e953-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4e953-119">Name</span></span>|<span data-ttu-id="4e953-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e953-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4e953-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e953-121">Authorization</span></span>|<span data-ttu-id="4e953-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e953-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4e953-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e953-124">Content-Type</span></span>|<span data-ttu-id="4e953-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e953-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e953-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e953-127">Request body</span></span>

<span data-ttu-id="4e953-128">No corpo da solicitação, forneça uma representação JSON do objeto [sitery](../resources/sitesource.md) .</span><span class="sxs-lookup"><span data-stu-id="4e953-128">In the request body, supply a JSON representation of the [siteSource](../resources/sitesource.md) object.</span></span>

<span data-ttu-id="4e953-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [site](../resources/sitesource.md).</span><span class="sxs-lookup"><span data-stu-id="4e953-129">The following table shows the properties that are required when you create the [siteSource](../resources/sitesource.md).</span></span>

|<span data-ttu-id="4e953-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e953-130">Property</span></span>|<span data-ttu-id="4e953-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e953-131">Type</span></span>|<span data-ttu-id="4e953-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e953-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e953-133">site@odata. bind</span><span class="sxs-lookup"><span data-stu-id="4e953-133">site@odata.bind</span></span>|<span data-ttu-id="4e953-134">String</span><span class="sxs-lookup"><span data-stu-id="4e953-134">String</span></span>|<span data-ttu-id="4e953-135">ID do site, que você pode obter do recurso de [site](../resources/site.md) usando o método [obter um recurso de site por caminho](../api/site-getbypath.md) .</span><span class="sxs-lookup"><span data-stu-id="4e953-135">ID of the site, which you can get from the [site](../resources/site.md) resource by using the [Get a site resource by path](../api/site-getbypath.md) method.</span></span> <span data-ttu-id="4e953-136">O uso é {nome_do_host}:/{Relative-Path}.</span><span class="sxs-lookup"><span data-stu-id="4e953-136">The usage is {hostname}:/{relative-path}.</span></span> <span data-ttu-id="4e953-137">Para a URL do site `https://contoso.sharepoint.com/sites/HumanResources` , a solicitação do Microsoft Graph seria `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` .</span><span class="sxs-lookup"><span data-stu-id="4e953-137">For the site URL `https://contoso.sharepoint.com/sites/HumanResources`, the Microsoft Graph request would be `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`.</span></span> <span data-ttu-id="4e953-138">O ID é o primeiro GUID listado no campo ID.</span><span class="sxs-lookup"><span data-stu-id="4e953-138">The ID is the first GUID listed in the ID field.</span></span>|

## <a name="response"></a><span data-ttu-id="4e953-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e953-139">Response</span></span>

<span data-ttu-id="4e953-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [sitery](../resources/sitesource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e953-140">If successful, this method returns a `201 Created` response code and a [siteSource](../resources/sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e953-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4e953-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4e953-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e953-142">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="4e953-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e953-143">Response</span></span>

<span data-ttu-id="4e953-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4e953-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
