---
title: Criar unifiedGroupSource
description: Crie um novo objeto unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6cfe9778de629538a51a0b6942754cb2e62593d2
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080390"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="048a0-103">Criar unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="048a0-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="048a0-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="048a0-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="048a0-105">Crie um novo [objeto unifiedGroupSource.](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="048a0-105">Create a new [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="048a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="048a0-106">Permissions</span></span>

<span data-ttu-id="048a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="048a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="048a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="048a0-109">Permission type</span></span>|<span data-ttu-id="048a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="048a0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="048a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="048a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="048a0-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="048a0-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="048a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="048a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="048a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="048a0-114">Not supported.</span></span>|
|<span data-ttu-id="048a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="048a0-115">Application</span></span>|<span data-ttu-id="048a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="048a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="048a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="048a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="048a0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="048a0-118">Request headers</span></span>

|<span data-ttu-id="048a0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="048a0-119">Name</span></span>|<span data-ttu-id="048a0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="048a0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="048a0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="048a0-121">Authorization</span></span>|<span data-ttu-id="048a0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="048a0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="048a0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="048a0-124">Content-Type</span></span>|<span data-ttu-id="048a0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="048a0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="048a0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="048a0-127">Request body</span></span>

<span data-ttu-id="048a0-128">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedGroupSource.](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="048a0-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="048a0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md).</span><span class="sxs-lookup"><span data-stu-id="048a0-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md).</span></span>

|<span data-ttu-id="048a0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="048a0-130">Property</span></span>|<span data-ttu-id="048a0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="048a0-131">Type</span></span>|<span data-ttu-id="048a0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="048a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="048a0-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="048a0-133">includedSources</span></span>|<span data-ttu-id="048a0-134">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="048a0-134">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="048a0-135">Especifica quais fontes estão incluídas neste grupo.</span><span class="sxs-lookup"><span data-stu-id="048a0-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="048a0-136">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="048a0-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="048a0-137">group@odata.bind</span><span class="sxs-lookup"><span data-stu-id="048a0-137">group@odata.bind</span></span>|<span data-ttu-id="048a0-138">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="048a0-138">String</span></span>|<span data-ttu-id="048a0-139">ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="048a0-139">ID of the group.</span></span> <span data-ttu-id="048a0-140">Para obter a ID do grupo, use a [operação Listar grupos.](../api/group-list.md)</span><span class="sxs-lookup"><span data-stu-id="048a0-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="048a0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="048a0-141">Response</span></span>

<span data-ttu-id="048a0-142">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="048a0-142">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="048a0-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="048a0-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="048a0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="048a0-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="048a0-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="048a0-145">HTTP</span></span>](#tab/http)
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
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84",
  "includedSources":  "mailbox, site"
}
```
# <a name="c"></a>[<span data-ttu-id="048a0-146">C#</span><span class="sxs-lookup"><span data-stu-id="048a0-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedgroupsource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="048a0-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="048a0-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedgroupsource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="048a0-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="048a0-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedgroupsource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="048a0-149">Java</span><span class="sxs-lookup"><span data-stu-id="048a0-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedgroupsource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="048a0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="048a0-150">Response</span></span>

> <span data-ttu-id="048a0-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="048a0-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('f4c0e095-d140-4392-bfe7-4e0ae637c566')/custodians('46363131333630303541423141324436')/unifiedGroupSources/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84",
    "displayName": "SFA Videos",
    "createdDateTime": "2021-03-31T21:22:57.0108027Z",
    "id": "33434233-3030-3739-3043-393039324633",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null
        }
    }
}
```
