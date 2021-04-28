---
title: Listar recursos do azureADDevice
description: Obter uma lista de objetos azureADDevice e suas propriedades.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: a3c77f5be32e37813fe08c61ca6b32432adf5c9c
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067774"
---
# <a name="list-azureaddevice-resources"></a><span data-ttu-id="c5a76-103">Listar recursos do azureADDevice</span><span class="sxs-lookup"><span data-stu-id="c5a76-103">List azureADDevice resources</span></span>
<span data-ttu-id="c5a76-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c5a76-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5a76-105">Obter uma lista de [objetos azureADDevice](../resources/windowsupdates-azureaddevice.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c5a76-105">Get a list of [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects and their properties.</span></span>

<span data-ttu-id="c5a76-106">Essa operação filtra o tipo de recurso totalmente `microsoft.graph.windowsUpdates.azureADDevice` qualificado, , que herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="c5a76-106">This operation filters on the fully qualified resource type, `microsoft.graph.windowsUpdates.azureADDevice`, which inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5a76-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5a76-107">Permissions</span></span>
<span data-ttu-id="c5a76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5a76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a76-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5a76-110">Permission type</span></span>|<span data-ttu-id="c5a76-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5a76-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a76-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5a76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5a76-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a76-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c5a76-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5a76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a76-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5a76-115">Not supported.</span></span>|
|<span data-ttu-id="c5a76-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5a76-116">Application</span></span>|<span data-ttu-id="c5a76-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a76-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a76-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5a76-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.azureADDevice')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5a76-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5a76-119">Optional query parameters</span></span>
<span data-ttu-id="c5a76-120">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="c5a76-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="c5a76-121">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="c5a76-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type.</span></span> <span data-ttu-id="c5a76-122">Por exemplo, para selecionar **a propriedade errors,** use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="c5a76-122">For example, to select the **errors** property, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5a76-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5a76-123">Request headers</span></span>
|<span data-ttu-id="c5a76-124">Nome</span><span class="sxs-lookup"><span data-stu-id="c5a76-124">Name</span></span>|<span data-ttu-id="c5a76-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5a76-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c5a76-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5a76-126">Authorization</span></span>|<span data-ttu-id="c5a76-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5a76-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a76-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5a76-129">Request body</span></span>
<span data-ttu-id="c5a76-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5a76-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5a76-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5a76-131">Response</span></span>

<span data-ttu-id="c5a76-132">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [azureADDevice](../resources/windowsupdates-azureaddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5a76-132">If successful, this method returns a `200 OK` response code and a collection of [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5a76-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5a76-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5a76-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5a76-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_azureaddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.azureADDevice')
```

### <a name="response"></a><span data-ttu-id="c5a76-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5a76-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.azureADDevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
      "errors": [],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
          "updateCategory": "feature"
        }
      ]
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "90b91efa-6d46-42cd-ad4d-381831773a85",
      "errors": [],
      "enrollments": []
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "0ee3eb63-caf3-44ce-9769-b83188cc683d",
      "errors": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
        }
      ],
      "enrollments": []
    }
  ]
}
```

