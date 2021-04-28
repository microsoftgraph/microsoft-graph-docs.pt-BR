---
title: Listar membros da audiência de implantação
description: Listar os recursos updatableAsset que são membros de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2ad3c2a2c4f47616e8064f6dddf7a09d095e615f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067250"
---
# <a name="list-deployment-audience-members"></a><span data-ttu-id="13865-103">Listar membros da audiência de implantação</span><span class="sxs-lookup"><span data-stu-id="13865-103">List deployment audience members</span></span>
<span data-ttu-id="13865-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="13865-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13865-105">Listar [os recursos updatableAsset](../resources/windowsupdates-updatableasset.md) que são membros de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="13865-105">List the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources that are members of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13865-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13865-106">Permissions</span></span>
<span data-ttu-id="13865-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13865-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13865-109">Permission type</span></span>|<span data-ttu-id="13865-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13865-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13865-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13865-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13865-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13865-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="13865-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13865-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13865-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13865-114">Not supported.</span></span>|
|<span data-ttu-id="13865-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13865-115">Application</span></span>|<span data-ttu-id="13865-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13865-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13865-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13865-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}/audience/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13865-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13865-118">Optional query parameters</span></span>
<span data-ttu-id="13865-119">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="13865-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="13865-120">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="13865-120">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="13865-121">Por exemplo, para selecionar [azureADDevice,](../resources/windowsupdates-azureaddevice.md) `errors` use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="13865-121">For example, to select [azureADDevice](../resources/windowsupdates-azureaddevice.md) `errors`, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13865-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13865-122">Request headers</span></span>
|<span data-ttu-id="13865-123">Nome</span><span class="sxs-lookup"><span data-stu-id="13865-123">Name</span></span>|<span data-ttu-id="13865-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="13865-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="13865-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="13865-125">Authorization</span></span>|<span data-ttu-id="13865-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13865-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13865-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13865-128">Request body</span></span>
<span data-ttu-id="13865-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13865-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13865-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="13865-130">Response</span></span>

<span data-ttu-id="13865-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13865-131">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13865-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13865-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13865-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13865-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/members
```


### <a name="response"></a><span data-ttu-id="13865-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="13865-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "fb95f07d-9e73-411d-99ab-7eca3a5122b1",
      "errors": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
        }
      ],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
        }
      ]
    },
  ]
}
```

