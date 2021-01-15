---
title: Obter custodian
description: Leia as propriedades e os relacionamentos de um objeto custodiante.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 8295767eb6b7ea4f7a1825b9b75d8b85c0eb525b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872636"
---
# <a name="get-custodian"></a><span data-ttu-id="555bb-103">Obter custodiatário</span><span class="sxs-lookup"><span data-stu-id="555bb-103">Get custodian</span></span>

<span data-ttu-id="555bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="555bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="555bb-105">Leia as propriedades e os relacionamentos de um [objeto custodiante.](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="555bb-105">Read the properties and relationships of a [custodian](../resources/custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="555bb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="555bb-106">Permissions</span></span>

<span data-ttu-id="555bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="555bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="555bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="555bb-109">Permission type</span></span>|<span data-ttu-id="555bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="555bb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="555bb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="555bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="555bb-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="555bb-112">User.Read</span></span>|
|<span data-ttu-id="555bb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="555bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="555bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="555bb-114">Not supported.</span></span>|
|<span data-ttu-id="555bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="555bb-115">Application</span></span>|<span data-ttu-id="555bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="555bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="555bb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="555bb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="555bb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="555bb-118">Optional query parameters</span></span>

<span data-ttu-id="555bb-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="555bb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="555bb-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="555bb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="555bb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="555bb-121">Request headers</span></span>

|<span data-ttu-id="555bb-122">Nome</span><span class="sxs-lookup"><span data-stu-id="555bb-122">Name</span></span>|<span data-ttu-id="555bb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="555bb-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="555bb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="555bb-124">Authorization</span></span>|<span data-ttu-id="555bb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="555bb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="555bb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="555bb-127">Request body</span></span>

<span data-ttu-id="555bb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="555bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="555bb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="555bb-129">Response</span></span>

<span data-ttu-id="555bb-130">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` objeto [custodiante](../resources/custodian.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="555bb-130">If successful, this method returns a `200 OK` response code and a [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="555bb-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="555bb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="555bb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="555bb-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="555bb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="555bb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custodian"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
```
# <a name="c"></a>[<span data-ttu-id="555bb-134">C#</span><span class="sxs-lookup"><span data-stu-id="555bb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="555bb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="555bb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="555bb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="555bb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="555bb-137">Java</span><span class="sxs-lookup"><span data-stu-id="555bb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="555bb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="555bb-138">Response</span></span>

<span data-ttu-id="555bb-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="555bb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": true,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T20:59:55.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
