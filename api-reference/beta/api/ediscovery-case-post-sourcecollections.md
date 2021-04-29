---
title: Criar sourceCollection
description: Crie um novo objeto sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 799601b3ca59c3522e4d023f7647bca523369659
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080311"
---
# <a name="create-sourcecollection"></a><span data-ttu-id="be36f-103">Criar sourceCollection</span><span class="sxs-lookup"><span data-stu-id="be36f-103">Create sourceCollection</span></span>

<span data-ttu-id="be36f-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="be36f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be36f-105">Crie um novo [objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="be36f-105">Create a new [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be36f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be36f-106">Permissions</span></span>

<span data-ttu-id="be36f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be36f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be36f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be36f-109">Permission type</span></span>|<span data-ttu-id="be36f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be36f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be36f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be36f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be36f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be36f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="be36f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be36f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be36f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be36f-114">Not supported.</span></span>|
|<span data-ttu-id="be36f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be36f-115">Application</span></span>|<span data-ttu-id="be36f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be36f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be36f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be36f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="request-headers"></a><span data-ttu-id="be36f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be36f-118">Request headers</span></span>

|<span data-ttu-id="be36f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="be36f-119">Name</span></span>|<span data-ttu-id="be36f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="be36f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="be36f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="be36f-121">Authorization</span></span>|<span data-ttu-id="be36f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be36f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="be36f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be36f-124">Content-Type</span></span>|<span data-ttu-id="be36f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be36f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be36f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be36f-127">Request body</span></span>

<span data-ttu-id="be36f-128">No corpo da solicitação, fornece uma representação JSON do [objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="be36f-128">In the request body, supply a JSON representation of the [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

<span data-ttu-id="be36f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [sourceCollection](../resources/ediscovery-sourcecollection.md).</span><span class="sxs-lookup"><span data-stu-id="be36f-129">The following table shows the properties that are required when you create the [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>

|<span data-ttu-id="be36f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be36f-130">Property</span></span>|<span data-ttu-id="be36f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="be36f-131">Type</span></span>|<span data-ttu-id="be36f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="be36f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be36f-133">dataSourceScopes</span><span class="sxs-lookup"><span data-stu-id="be36f-133">dataSourceScopes</span></span>|<span data-ttu-id="be36f-134">microsoft.graph.ediscovery.dataSourceScopes</span><span class="sxs-lookup"><span data-stu-id="be36f-134">microsoft.graph.ediscovery.dataSourceScopes</span></span>|<span data-ttu-id="be36f-135">Quando especificado, a coleção se estenderá por um serviço para uma carga de trabalho inteira.</span><span class="sxs-lookup"><span data-stu-id="be36f-135">When specified, the collection will span across a service for an entire workload.</span></span> <span data-ttu-id="be36f-136">Os valores possíveis são: `none` , , , , `allTenantMailboxes` `allTenantSites` `allCaseCustodians` `allCaseNoncustodialDataSources` .</span><span class="sxs-lookup"><span data-stu-id="be36f-136">Possible values are: `none`,`allTenantMailboxes`,`allTenantSites`,`allCaseCustodians`,`allCaseNoncustodialDataSources`.</span></span> <span data-ttu-id="be36f-137">**Observação:** Um custodiante ou a especificação de dadosSourceScope é necessária ao criar uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="be36f-137">**Note:** Either one custodian or specifying dataSourceScope is required when creating a source collection.</span></span>|
|<span data-ttu-id="be36f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="be36f-138">displayName</span></span>|<span data-ttu-id="be36f-139">String</span><span class="sxs-lookup"><span data-stu-id="be36f-139">String</span></span>|<span data-ttu-id="be36f-140">O nome de exibição da **sourceCollection**</span><span class="sxs-lookup"><span data-stu-id="be36f-140">The display name of the **sourceCollection**</span></span>|
|<span data-ttu-id="be36f-141">custodianSources</span><span class="sxs-lookup"><span data-stu-id="be36f-141">custodianSources</span></span>|<span data-ttu-id="be36f-142">[coleção microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="be36f-142">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="be36f-143">As fontes custodiadas a incluir nesta pesquisa.</span><span class="sxs-lookup"><span data-stu-id="be36f-143">The custodian sources to include in this search.</span></span> <span data-ttu-id="be36f-144">Você pode obter a URL do [site custodianteSources,](../api/ediscovery-custodian-list-sitesources.md) [unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)ou [userSources](../api/ediscovery-custodian-list-usersources.md) mais a ID da origem.</span><span class="sxs-lookup"><span data-stu-id="be36f-144">You can get the URL from from custodian [siteSources](../api/ediscovery-custodian-list-sitesources.md), [unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md), or [userSources](../api/ediscovery-custodian-list-usersources.md) plus the ID of the source.</span></span> <span data-ttu-id="be36f-145">**Observação:** Um custodiante ou a especificação da origem do locatário é necessário ao criar uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="be36f-145">**Note:** Either one custodian or specifying tenant source is required when creating a source collection.</span></span> |

## <a name="response"></a><span data-ttu-id="be36f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="be36f-146">Response</span></span>

<span data-ttu-id="be36f-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be36f-147">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be36f-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be36f-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be36f-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be36f-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="be36f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="be36f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sourcecollection_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections
Content-Type: application/json
Content-length: 272

{
    "displayName": "Quarterly Financials search",
    "contentQuery": "subject:'Quarterly Financials'",
    "custodianSources@odata.bind": [
        "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735"
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="be36f-151">C#</span><span class="sxs-lookup"><span data-stu-id="be36f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sourcecollection-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be36f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be36f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sourcecollection-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be36f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be36f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sourcecollection-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be36f-154">Java</span><span class="sxs-lookup"><span data-stu-id="be36f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sourcecollection-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be36f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="be36f-155">Response</span></span>

> <span data-ttu-id="be36f-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="be36f-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "dataSourceScopes": "none",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    }
}
```
