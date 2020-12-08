---
title: Criar unifiedGroupSource
description: Criar um novo objeto unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f92fa2454b7ab20946091784af11b23ef2252acc
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597480"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="3e515-103">Criar unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="3e515-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="3e515-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3e515-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e515-105">Criar um novo objeto [unifiedGroupSource](../resources/unifiedgroupsource.md) .</span><span class="sxs-lookup"><span data-stu-id="3e515-105">Create a new [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e515-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3e515-106">Permissions</span></span>

<span data-ttu-id="3e515-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e515-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e515-109">Permission type</span></span>|<span data-ttu-id="3e515-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e515-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e515-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e515-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e515-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="3e515-112">User.Read</span></span>|
|<span data-ttu-id="3e515-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e515-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e515-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e515-114">Not supported.</span></span>|
|<span data-ttu-id="3e515-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e515-115">Application</span></span>|<span data-ttu-id="3e515-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e515-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e515-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e515-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="3e515-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e515-118">Request headers</span></span>

|<span data-ttu-id="3e515-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3e515-119">Name</span></span>|<span data-ttu-id="3e515-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e515-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3e515-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e515-121">Authorization</span></span>|<span data-ttu-id="3e515-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e515-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3e515-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e515-124">Content-Type</span></span>|<span data-ttu-id="3e515-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e515-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e515-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e515-127">Request body</span></span>

<span data-ttu-id="3e515-128">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedGroupSource](../resources/unifiedgroupsource.md) .</span><span class="sxs-lookup"><span data-stu-id="3e515-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="3e515-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [unifiedGroupSource](../resources/unifiedgroupsource.md).</span><span class="sxs-lookup"><span data-stu-id="3e515-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/unifiedgroupsource.md).</span></span>

|<span data-ttu-id="3e515-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e515-130">Property</span></span>|<span data-ttu-id="3e515-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e515-131">Type</span></span>|<span data-ttu-id="3e515-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e515-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e515-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="3e515-133">includedSources</span></span>|<span data-ttu-id="3e515-134">sourceType</span><span class="sxs-lookup"><span data-stu-id="3e515-134">sourceType</span></span>|<span data-ttu-id="3e515-135">Especifica quais fontes são incluídas nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="3e515-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="3e515-136">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="3e515-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="3e515-137">group@odata. bind</span><span class="sxs-lookup"><span data-stu-id="3e515-137">group@odata.bind</span></span>|<span data-ttu-id="3e515-138">String</span><span class="sxs-lookup"><span data-stu-id="3e515-138">String</span></span>|<span data-ttu-id="3e515-139">ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="3e515-139">ID of the group.</span></span> <span data-ttu-id="3e515-140">Para obter a ID de grupo, use a operação de [grupos de listas](../api/group-list.md) .</span><span class="sxs-lookup"><span data-stu-id="3e515-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="3e515-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e515-141">Response</span></span>

<span data-ttu-id="3e515-142">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [unifiedGroupSource](../resources/unifiedgroupsource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e515-142">If successful, this method returns a `201 Created` response code and a [unifiedGroupSource](../resources/unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e515-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3e515-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e515-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e515-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
Content-Type: application/json
Content-length: 219

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site"
}
```

### <a name="response"></a><span data-ttu-id="3e515-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e515-145">Response</span></span>

<span data-ttu-id="3e515-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3e515-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedGroupSource"
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
