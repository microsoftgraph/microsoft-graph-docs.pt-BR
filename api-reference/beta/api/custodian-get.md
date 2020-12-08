---
title: Obter os responsáveis
description: Leia as propriedades e os relacionamentos de um objeto de responsáveis.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: a2829d0c74de6482a4a32eea38735b35b025e711
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597492"
---
# <a name="get-custodian"></a><span data-ttu-id="fbecf-103">Obter os responsáveis</span><span class="sxs-lookup"><span data-stu-id="fbecf-103">Get custodian</span></span>

<span data-ttu-id="fbecf-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fbecf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbecf-105">Leia as propriedades e os relacionamentos de um objeto de [responsáveis](../resources/custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="fbecf-105">Read the properties and relationships of a [custodian](../resources/custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbecf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fbecf-106">Permissions</span></span>

<span data-ttu-id="fbecf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbecf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbecf-109">Permission type</span></span>|<span data-ttu-id="fbecf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbecf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbecf-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbecf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbecf-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="fbecf-112">User.Read</span></span>|
|<span data-ttu-id="fbecf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbecf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbecf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbecf-114">Not supported.</span></span>|
|<span data-ttu-id="fbecf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbecf-115">Application</span></span>|<span data-ttu-id="fbecf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbecf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbecf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbecf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbecf-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fbecf-118">Optional query parameters</span></span>

<span data-ttu-id="fbecf-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fbecf-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fbecf-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fbecf-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbecf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbecf-121">Request headers</span></span>

|<span data-ttu-id="fbecf-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fbecf-122">Name</span></span>|<span data-ttu-id="fbecf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbecf-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fbecf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbecf-124">Authorization</span></span>|<span data-ttu-id="fbecf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbecf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbecf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbecf-127">Request body</span></span>

<span data-ttu-id="fbecf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbecf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbecf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbecf-129">Response</span></span>

<span data-ttu-id="fbecf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [responsáveis](../resources/custodian.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbecf-130">If successful, this method returns a `200 OK` response code and a [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fbecf-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fbecf-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fbecf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbecf-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_custodian"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
```

### <a name="response"></a><span data-ttu-id="fbecf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbecf-133">Response</span></span>

<span data-ttu-id="fbecf-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fbecf-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
