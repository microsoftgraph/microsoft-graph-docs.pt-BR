---
title: Listar unifiedGroupSources
description: Obtenha uma lista dos objetos unifiedGroupSource e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: d83364b2034036c7a0e4cf0ec1097a54645a52a1
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597490"
---
# <a name="list-unifiedgroupsources"></a><span data-ttu-id="38187-103">Listar unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="38187-103">List unifiedGroupSources</span></span>

<span data-ttu-id="38187-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="38187-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38187-105">Obtenha uma lista dos objetos [unifiedGroupSource](../resources/unifiedgroupsource.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="38187-105">Get a list of the [unifiedGroupSource](../resources/unifiedgroupsource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="38187-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="38187-106">Permissions</span></span>

<span data-ttu-id="38187-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38187-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38187-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38187-109">Permission type</span></span>|<span data-ttu-id="38187-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38187-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38187-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38187-111">Delegated (work or school account)</span></span>|<span data-ttu-id="38187-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="38187-112">User.Read</span></span>|
|<span data-ttu-id="38187-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38187-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38187-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38187-114">Not supported.</span></span>|
|<span data-ttu-id="38187-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38187-115">Application</span></span>|<span data-ttu-id="38187-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38187-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38187-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38187-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38187-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="38187-118">Optional query parameters</span></span>

<span data-ttu-id="38187-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38187-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="38187-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="38187-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="38187-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38187-121">Request headers</span></span>

|<span data-ttu-id="38187-122">Nome</span><span class="sxs-lookup"><span data-stu-id="38187-122">Name</span></span>|<span data-ttu-id="38187-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="38187-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="38187-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="38187-124">Authorization</span></span>|<span data-ttu-id="38187-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38187-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38187-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38187-127">Request body</span></span>

<span data-ttu-id="38187-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38187-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38187-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="38187-129">Response</span></span>

<span data-ttu-id="38187-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [unifiedGroupSource](../resources/unifiedgroupsource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38187-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedGroupSource](../resources/unifiedgroupsource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38187-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="38187-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38187-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38187-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedgroupsource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

### <a name="response"></a><span data-ttu-id="38187-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="38187-133">Response</span></span>

<span data-ttu-id="38187-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="38187-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedGroupSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
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
    ]
}
```
