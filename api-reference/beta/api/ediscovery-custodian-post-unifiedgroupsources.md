---
title: Criar unifiedGroupSource
description: Crie um novo objeto unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 96e97475c41c983c38f3d8be5c2ec95315427c7f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773239"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="657d1-103">Criar unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="657d1-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="657d1-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="657d1-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="657d1-105">Crie um novo [objeto unifiedGroupSource.](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="657d1-105">Create a new [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="657d1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="657d1-106">Permissions</span></span>

<span data-ttu-id="657d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="657d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="657d1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="657d1-109">Permission type</span></span>|<span data-ttu-id="657d1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="657d1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="657d1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="657d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="657d1-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="657d1-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="657d1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="657d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="657d1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="657d1-114">Not supported.</span></span>|
|<span data-ttu-id="657d1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="657d1-115">Application</span></span>|<span data-ttu-id="657d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="657d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="657d1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="657d1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="657d1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="657d1-118">Request headers</span></span>

|<span data-ttu-id="657d1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="657d1-119">Name</span></span>|<span data-ttu-id="657d1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="657d1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="657d1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="657d1-121">Authorization</span></span>|<span data-ttu-id="657d1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="657d1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="657d1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="657d1-124">Content-Type</span></span>|<span data-ttu-id="657d1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="657d1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="657d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="657d1-127">Request body</span></span>

<span data-ttu-id="657d1-128">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedGroupSource.](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="657d1-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="657d1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md).</span><span class="sxs-lookup"><span data-stu-id="657d1-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md).</span></span>

|<span data-ttu-id="657d1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="657d1-130">Property</span></span>|<span data-ttu-id="657d1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="657d1-131">Type</span></span>|<span data-ttu-id="657d1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="657d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="657d1-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="657d1-133">includedSources</span></span>|<span data-ttu-id="657d1-134">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="657d1-134">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="657d1-135">Especifica quais fontes estão incluídas neste grupo.</span><span class="sxs-lookup"><span data-stu-id="657d1-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="657d1-136">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="657d1-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="657d1-137">group@odata.bind</span><span class="sxs-lookup"><span data-stu-id="657d1-137">group@odata.bind</span></span>|<span data-ttu-id="657d1-138">String</span><span class="sxs-lookup"><span data-stu-id="657d1-138">String</span></span>|<span data-ttu-id="657d1-139">ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="657d1-139">ID of the group.</span></span> <span data-ttu-id="657d1-140">Para obter a ID do grupo, use a [operação Listar grupos.](../api/group-list.md)</span><span class="sxs-lookup"><span data-stu-id="657d1-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="657d1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="657d1-141">Response</span></span>

<span data-ttu-id="657d1-142">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="657d1-142">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="657d1-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="657d1-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="657d1-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="657d1-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="657d1-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="657d1-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="657d1-146">C#</span><span class="sxs-lookup"><span data-stu-id="657d1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedgroupsource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="657d1-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="657d1-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedgroupsource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="657d1-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="657d1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedgroupsource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="657d1-149">Java</span><span class="sxs-lookup"><span data-stu-id="657d1-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedgroupsource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="657d1-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="657d1-150">Response</span></span>

<span data-ttu-id="657d1-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="657d1-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
