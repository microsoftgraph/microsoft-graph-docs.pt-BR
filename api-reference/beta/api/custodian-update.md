---
title: Atualizar custodian
description: Atualizar as propriedades de um objeto custodiante.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: bae5be0c8712735f0a7c369f3ec79146a1608acf
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872489"
---
# <a name="update-custodian"></a><span data-ttu-id="02a79-103">Atualizar custodian</span><span class="sxs-lookup"><span data-stu-id="02a79-103">Update custodian</span></span>

<span data-ttu-id="02a79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02a79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a79-105">Atualizar as propriedades de [um objeto custodiante.](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="02a79-105">Update the properties of a [custodian](../resources/custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02a79-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02a79-106">Permissions</span></span>

<span data-ttu-id="02a79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02a79-109">Permission type</span></span>|<span data-ttu-id="02a79-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02a79-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02a79-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02a79-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="02a79-112">User.Read</span></span>|
|<span data-ttu-id="02a79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02a79-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02a79-114">Not supported.</span></span>|
|<span data-ttu-id="02a79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02a79-115">Application</span></span>|<span data-ttu-id="02a79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02a79-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02a79-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}
```

## <a name="request-headers"></a><span data-ttu-id="02a79-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02a79-118">Request headers</span></span>

|<span data-ttu-id="02a79-119">Nome</span><span class="sxs-lookup"><span data-stu-id="02a79-119">Name</span></span>|<span data-ttu-id="02a79-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="02a79-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02a79-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="02a79-121">Authorization</span></span>|<span data-ttu-id="02a79-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02a79-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="02a79-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02a79-124">Content-Type</span></span>|<span data-ttu-id="02a79-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02a79-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02a79-127">Request body</span></span>

<span data-ttu-id="02a79-128">No corpo da solicitação, fornece uma representação JSON do [objeto custodiante.](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="02a79-128">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="02a79-129">A tabela a seguir lista as propriedades de [um objeto custodiante](../resources/custodian.md) que pode ser modificado.</span><span class="sxs-lookup"><span data-stu-id="02a79-129">The following table lists the properties of a [custodian](../resources/custodian.md) object that can be modified.</span></span>

|<span data-ttu-id="02a79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02a79-130">Property</span></span>|<span data-ttu-id="02a79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02a79-131">Type</span></span>|<span data-ttu-id="02a79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02a79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a79-133">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="02a79-133">applyHoldToSources</span></span>|<span data-ttu-id="02a79-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="02a79-134">Boolean</span></span>|<span data-ttu-id="02a79-135">Identifica se as fontes de um custodiador foram colocadas em espera durante a criação.</span><span class="sxs-lookup"><span data-stu-id="02a79-135">Identifies whether a custodian's sources were placed on hold during creation.</span></span> <span data-ttu-id="02a79-136">Para obter detalhes, [consulte Colocar custodiantes em espera.](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold)</span><span class="sxs-lookup"><span data-stu-id="02a79-136">For details, see [Place custodians on hold](/microsoft-365/compliance/add-custodians-to-case#step-4-place-custodians-on-hold).</span></span>|

## <a name="response"></a><span data-ttu-id="02a79-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="02a79-137">Response</span></span>

<span data-ttu-id="02a79-138">Se bem-sucedido, este método retorna um código `200 OK` de resposta e um objeto [custodiante](../resources/custodian.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02a79-138">If successful, this method returns a `200 OK` response code and an updated [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02a79-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02a79-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02a79-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02a79-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="02a79-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="02a79-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="02a79-142">C#</span><span class="sxs-lookup"><span data-stu-id="02a79-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02a79-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02a79-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02a79-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02a79-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02a79-145">Java</span><span class="sxs-lookup"><span data-stu-id="02a79-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02a79-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="02a79-146">Response</span></span>

<span data-ttu-id="02a79-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02a79-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
