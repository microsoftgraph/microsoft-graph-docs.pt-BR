---
title: Obter azureADDevice
description: Leia as propriedades de um objeto azureADDevice.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 22cf7a45e2782ee1a012e2ff1f02a94e9ff20401
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067823"
---
# <a name="get-azureaddevice"></a><span data-ttu-id="682cd-103">Obter azureADDevice</span><span class="sxs-lookup"><span data-stu-id="682cd-103">Get azureADDevice</span></span>
<span data-ttu-id="682cd-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="682cd-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="682cd-105">Leia as propriedades de um [objeto azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="682cd-105">Read the properties of an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="682cd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="682cd-106">Permissions</span></span>
<span data-ttu-id="682cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="682cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="682cd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="682cd-109">Permission type</span></span>|<span data-ttu-id="682cd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="682cd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="682cd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="682cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="682cd-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682cd-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="682cd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="682cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="682cd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="682cd-114">Not supported.</span></span>|
|<span data-ttu-id="682cd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="682cd-115">Application</span></span>|<span data-ttu-id="682cd-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682cd-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="682cd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="682cd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="682cd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="682cd-118">Optional query parameters</span></span>
<span data-ttu-id="682cd-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="682cd-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="682cd-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="682cd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="682cd-121">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="682cd-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type.</span></span> <span data-ttu-id="682cd-122">Por exemplo, para selecionar **a propriedade errors,** use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="682cd-122">For example, to select the **errors** property, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="682cd-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="682cd-123">Request headers</span></span>
|<span data-ttu-id="682cd-124">Nome</span><span class="sxs-lookup"><span data-stu-id="682cd-124">Name</span></span>|<span data-ttu-id="682cd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="682cd-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="682cd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="682cd-126">Authorization</span></span>|<span data-ttu-id="682cd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="682cd-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="682cd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="682cd-129">Request body</span></span>
<span data-ttu-id="682cd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="682cd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="682cd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="682cd-131">Response</span></span>

<span data-ttu-id="682cd-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto azureADDevice](../resources/windowsupdates-azureaddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="682cd-132">If successful, this method returns a `200 OK` response code and an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="682cd-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="682cd-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="682cd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="682cd-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_azureaddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```

### <a name="response"></a><span data-ttu-id="682cd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="682cd-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

