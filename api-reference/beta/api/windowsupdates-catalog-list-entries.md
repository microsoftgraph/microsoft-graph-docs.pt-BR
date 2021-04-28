---
title: Listar entradas
description: Obter uma lista de recursos catalogEntry do catálogo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: c00dafaf9c6a28f5dd5c747a747ab1d8e84419a4
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067806"
---
# <a name="list-entries"></a><span data-ttu-id="b7326-103">Listar entradas</span><span class="sxs-lookup"><span data-stu-id="b7326-103">List entries</span></span>
<span data-ttu-id="b7326-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b7326-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7326-105">Obter uma lista de [recursos catalogEntry](../resources/windowsupdates-catalogentry.md) do [catálogo](../resources/windowsupdates-catalog.md).</span><span class="sxs-lookup"><span data-stu-id="b7326-105">Get a list of [catalogEntry](../resources/windowsupdates-catalogentry.md) resources from the [catalog](../resources/windowsupdates-catalog.md).</span></span>

<span data-ttu-id="b7326-106">Atualmente, essa operação retorna entradas dos tipos [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) ou [qualityUpdateCatalog,](../resources/windowsupdates-qualityupdatecatalogentry.md) herdados de **catalogEntry**.</span><span class="sxs-lookup"><span data-stu-id="b7326-106">Currently, this operation returns entries of the [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) or [qualityUpdateCatalog](../resources/windowsupdates-qualityupdatecatalogentry.md) types, inherited from **catalogEntry**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b7326-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7326-107">Permissions</span></span>
<span data-ttu-id="b7326-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7326-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7326-110">Permission type</span></span>|<span data-ttu-id="b7326-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7326-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7326-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7326-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7326-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7326-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="b7326-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7326-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7326-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7326-115">Not supported.</span></span>|
|<span data-ttu-id="b7326-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7326-116">Application</span></span>|<span data-ttu-id="b7326-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7326-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7326-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7326-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/catalog/entries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7326-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b7326-119">Optional query parameters</span></span>
<span data-ttu-id="b7326-120">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="b7326-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="b7326-121">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de **catalogEntry**, inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="b7326-121">To use a query parameter on a property that is not inherited from **catalogEntry**, include the full resource type for the property.</span></span> <span data-ttu-id="b7326-122">Por exemplo, para filtrar na propriedade **version** [de featureUpdateCatalogEntry,](../resources/windowsupdates-featureupdatecatalogentry.md)use `$filter=microsoft.graph.windowsUpdates.featureUpdateCatalogEntry/version` .</span><span class="sxs-lookup"><span data-stu-id="b7326-122">For example, to filter on the **version** property of [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), use `$filter=microsoft.graph.windowsUpdates.featureUpdateCatalogEntry/version`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7326-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7326-123">Request headers</span></span>
|<span data-ttu-id="b7326-124">Nome</span><span class="sxs-lookup"><span data-stu-id="b7326-124">Name</span></span>|<span data-ttu-id="b7326-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7326-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b7326-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7326-126">Authorization</span></span>|<span data-ttu-id="b7326-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7326-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7326-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7326-129">Request body</span></span>
<span data-ttu-id="b7326-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7326-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7326-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7326-131">Response</span></span>

<span data-ttu-id="b7326-132">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos catalogEntry no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7326-132">If successful, this method returns a `200 OK` response code and a collection of catalogEntry objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7326-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7326-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7326-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7326-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_catalogentry"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries
```


### <a name="response"></a><span data-ttu-id="b7326-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7326-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.catalogEntry)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
      "id": "c1dec151-c151-c1de-51c1-dec151c1dec1",
      "displayName": "String",
      "releaseDateTime": "String (timestamp)",
      "deployableUntilDateTime": "String (timestamp)",
      "version": "String"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
      "id": "d0c03fbb-43b9-4dff-840b-974ef227384d",
      "displayName": "String",
      "releaseDateTime": "String (timestamp)",
      "deployableUntilDateTime": "String (timestamp)",
      "isExpeditable": true,
      "qualityUpdateClassification": "security"
    }
  ]
}
```

