---
title: Criar unifiedGroupSource
description: Crie um novo objeto unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1c2ffe7ca2739b728cd15561266ee583e98b320e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445802"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="4edeb-103">Criar unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="4edeb-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="4edeb-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4edeb-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4edeb-105">Crie um novo [objeto unifiedGroupSource.](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="4edeb-105">Create a new [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4edeb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4edeb-106">Permissions</span></span>

<span data-ttu-id="4edeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4edeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4edeb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4edeb-109">Permission type</span></span>|<span data-ttu-id="4edeb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4edeb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4edeb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4edeb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4edeb-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4edeb-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="4edeb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4edeb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4edeb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4edeb-114">Not supported.</span></span>|
|<span data-ttu-id="4edeb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4edeb-115">Application</span></span>|<span data-ttu-id="4edeb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4edeb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4edeb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4edeb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="4edeb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4edeb-118">Request headers</span></span>

|<span data-ttu-id="4edeb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4edeb-119">Name</span></span>|<span data-ttu-id="4edeb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4edeb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4edeb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4edeb-121">Authorization</span></span>|<span data-ttu-id="4edeb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4edeb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4edeb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4edeb-124">Content-Type</span></span>|<span data-ttu-id="4edeb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4edeb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4edeb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4edeb-127">Request body</span></span>

<span data-ttu-id="4edeb-128">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedGroupSource.](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="4edeb-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="4edeb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md).</span><span class="sxs-lookup"><span data-stu-id="4edeb-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md).</span></span>

|<span data-ttu-id="4edeb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4edeb-130">Property</span></span>|<span data-ttu-id="4edeb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4edeb-131">Type</span></span>|<span data-ttu-id="4edeb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4edeb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4edeb-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="4edeb-133">includedSources</span></span>|<span data-ttu-id="4edeb-134">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="4edeb-134">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="4edeb-135">Especifica quais fontes estão incluídas neste grupo.</span><span class="sxs-lookup"><span data-stu-id="4edeb-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="4edeb-136">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="4edeb-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="4edeb-137">group@odata.bind</span><span class="sxs-lookup"><span data-stu-id="4edeb-137">group@odata.bind</span></span>|<span data-ttu-id="4edeb-138">String</span><span class="sxs-lookup"><span data-stu-id="4edeb-138">String</span></span>|<span data-ttu-id="4edeb-139">ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="4edeb-139">ID of the group.</span></span> <span data-ttu-id="4edeb-140">Para obter a ID do grupo, use a [operação Listar grupos.](../api/group-list.md)</span><span class="sxs-lookup"><span data-stu-id="4edeb-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="4edeb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4edeb-141">Response</span></span>

<span data-ttu-id="4edeb-142">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4edeb-142">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4edeb-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4edeb-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4edeb-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4edeb-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources
Content-Type: application/json
Content-length: 219

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site"
}
```

### <a name="response"></a><span data-ttu-id="4edeb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4edeb-145">Response</span></span>

<span data-ttu-id="4edeb-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4edeb-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site",
  "id": "14202dd90a1f4ccc84929586326c7104",
  "displayName": "SFA Videos",
  "createdDateTime": "2020-03-13T22:38:00.8985662Z",
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Megan Bowen"
      }
  }
}
```
