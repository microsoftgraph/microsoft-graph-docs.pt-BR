---
title: Obter unifiedGroupSource
description: Leia as propriedades e os relacionamentos de um objeto unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f3867c3c649865d34f225dc2bd928aa1067b4f55
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597526"
---
# <a name="get-unifiedgroupsource"></a><span data-ttu-id="55ae2-103">Obter unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="55ae2-103">Get unifiedGroupSource</span></span>

<span data-ttu-id="55ae2-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="55ae2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55ae2-105">Leia as propriedades e os relacionamentos de um objeto [unifiedGroupSource](../resources/unifiedgroupsource.md) .</span><span class="sxs-lookup"><span data-stu-id="55ae2-105">Read the properties and relationships of a [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55ae2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="55ae2-106">Permissions</span></span>

<span data-ttu-id="55ae2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55ae2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55ae2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55ae2-109">Permission type</span></span>|<span data-ttu-id="55ae2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55ae2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55ae2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55ae2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55ae2-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="55ae2-112">User.Read</span></span>|
|<span data-ttu-id="55ae2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55ae2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55ae2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55ae2-114">Not supported.</span></span>|
|<span data-ttu-id="55ae2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55ae2-115">Application</span></span>|<span data-ttu-id="55ae2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55ae2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55ae2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55ae2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55ae2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55ae2-118">Optional query parameters</span></span>

<span data-ttu-id="55ae2-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55ae2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="55ae2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="55ae2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="55ae2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55ae2-121">Request headers</span></span>

|<span data-ttu-id="55ae2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="55ae2-122">Name</span></span>|<span data-ttu-id="55ae2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="55ae2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="55ae2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="55ae2-124">Authorization</span></span>|<span data-ttu-id="55ae2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55ae2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55ae2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55ae2-127">Request body</span></span>

<span data-ttu-id="55ae2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55ae2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55ae2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="55ae2-129">Response</span></span>

<span data-ttu-id="55ae2-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [unifiedGroupSource](../resources/unifiedgroupsource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55ae2-130">If successful, this method returns a `200 OK` response code and a [unifiedGroupSource](../resources/unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55ae2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55ae2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55ae2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55ae2-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedgroupsource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

### <a name="response"></a><span data-ttu-id="55ae2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="55ae2-133">Response</span></span>

<span data-ttu-id="55ae2-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55ae2-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedGroupSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "displayName": "Developers group",
    "createdDateTime": "2020-10-27T15:14:11.0048392Z",
    "id": "33434233-3030-3739-3043-393039324633",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "Megan Bowen"
        }
    }
}
```
