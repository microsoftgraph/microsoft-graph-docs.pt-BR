---
title: Atualizar responsáveis
description: Atualizar as propriedades de um objeto de responsáveis.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 605438ac3ba9883ca159fe97015701282f39e347
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658901"
---
# <a name="update-custodian"></a><span data-ttu-id="818e4-103">Atualizar responsáveis</span><span class="sxs-lookup"><span data-stu-id="818e4-103">Update custodian</span></span>

<span data-ttu-id="818e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="818e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="818e4-105">Atualizar as propriedades de um objeto de [responsáveis](../resources/custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="818e4-105">Update the properties of a [custodian](../resources/custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="818e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="818e4-106">Permissions</span></span>

<span data-ttu-id="818e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="818e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="818e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="818e4-109">Permission type</span></span>|<span data-ttu-id="818e4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="818e4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="818e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="818e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="818e4-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="818e4-112">User.Read</span></span>|
|<span data-ttu-id="818e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="818e4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="818e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="818e4-114">Not supported.</span></span>|
|<span data-ttu-id="818e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="818e4-115">Application</span></span>|<span data-ttu-id="818e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="818e4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="818e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="818e4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}
```

## <a name="request-headers"></a><span data-ttu-id="818e4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="818e4-118">Request headers</span></span>

|<span data-ttu-id="818e4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="818e4-119">Name</span></span>|<span data-ttu-id="818e4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="818e4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="818e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="818e4-121">Authorization</span></span>|<span data-ttu-id="818e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="818e4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="818e4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="818e4-124">Content-Type</span></span>|<span data-ttu-id="818e4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="818e4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="818e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="818e4-127">Request body</span></span>

<span data-ttu-id="818e4-128">No corpo da solicitação, forneça uma representação JSON do objeto [responsáveis](../resources/custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="818e4-128">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="818e4-129">A tabela a seguir lista as propriedades de um objeto [responsáveis](../resources/custodian.md) que podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="818e4-129">The following table lists the properties of a [custodian](../resources/custodian.md) object that can be modified.</span></span>

|<span data-ttu-id="818e4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="818e4-130">Property</span></span>|<span data-ttu-id="818e4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="818e4-131">Type</span></span>|<span data-ttu-id="818e4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="818e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="818e4-133">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="818e4-133">applyHoldToSources</span></span>|<span data-ttu-id="818e4-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="818e4-134">Boolean</span></span>|<span data-ttu-id="818e4-135">Identifica se as fontes dos responsáveis foram colocadas em espera durante a criação.</span><span class="sxs-lookup"><span data-stu-id="818e4-135">Identifies whether a custodian's sources were placed on hold during creation.</span></span> <span data-ttu-id="818e4-136">Para obter detalhes, consulte [colocar os responsáveis em espera](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold).</span><span class="sxs-lookup"><span data-stu-id="818e4-136">For details, see [Place custodians on hold](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold).</span></span>|

## <a name="response"></a><span data-ttu-id="818e4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="818e4-137">Response</span></span>

<span data-ttu-id="818e4-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [responsáveis](../resources/custodian.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="818e4-138">If successful, this method returns a `200 OK` response code and an updated [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="818e4-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="818e4-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="818e4-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="818e4-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="818e4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="818e4-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_custodian"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
Content-Type: application/json
Content-length: 254

{
  "applyHoldToSources": "false",
}
```
# <a name="c"></a>[<span data-ttu-id="818e4-142">C#</span><span class="sxs-lookup"><span data-stu-id="818e4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="818e4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="818e4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="818e4-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="818e4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="818e4-145">Java</span><span class="sxs-lookup"><span data-stu-id="818e4-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="818e4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="818e4-146">Response</span></span>

<span data-ttu-id="818e4-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="818e4-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T21:01:34.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
