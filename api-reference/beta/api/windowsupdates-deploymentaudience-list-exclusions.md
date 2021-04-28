---
title: Listar exclusões de audiência de implantação
description: Listar os recursos updatableAsset excluídos de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 6f65aa86694478a545c236b7cd4f54a9468bb601
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067249"
---
# <a name="list-deployment-audience-exclusions"></a><span data-ttu-id="ac2b2-103">Listar exclusões de audiência de implantação</span><span class="sxs-lookup"><span data-stu-id="ac2b2-103">List deployment audience exclusions</span></span>
<span data-ttu-id="ac2b2-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ac2b2-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac2b2-105">Listar [os recursos updatableAsset](../resources/windowsupdates-updatableasset.md) excluídos de uma [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="ac2b2-105">List the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources that are excluded from a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac2b2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac2b2-106">Permissions</span></span>
<span data-ttu-id="ac2b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac2b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac2b2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac2b2-109">Permission type</span></span>|<span data-ttu-id="ac2b2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac2b2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac2b2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac2b2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac2b2-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac2b2-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="ac2b2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac2b2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac2b2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac2b2-114">Not supported.</span></span>|
|<span data-ttu-id="ac2b2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac2b2-115">Application</span></span>|<span data-ttu-id="ac2b2-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac2b2-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac2b2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac2b2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}/audience/exclusions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac2b2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac2b2-118">Optional query parameters</span></span>
<span data-ttu-id="ac2b2-119">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="ac2b2-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="ac2b2-120">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="ac2b2-120">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="ac2b2-121">Por exemplo, para selecionar [azureADDevice,](../resources/windowsupdates-azureaddevice.md) `errors` use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="ac2b2-121">For example, to select [azureADDevice](../resources/windowsupdates-azureaddevice.md) `errors`, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ac2b2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac2b2-122">Request headers</span></span>
|<span data-ttu-id="ac2b2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ac2b2-123">Name</span></span>|<span data-ttu-id="ac2b2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac2b2-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac2b2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac2b2-125">Authorization</span></span>|<span data-ttu-id="ac2b2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac2b2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac2b2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac2b2-128">Request body</span></span>
<span data-ttu-id="ac2b2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac2b2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac2b2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac2b2-130">Response</span></span>

<span data-ttu-id="ac2b2-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac2b2-131">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac2b2-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ac2b2-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac2b2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac2b2-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/exclusions
```


### <a name="response"></a><span data-ttu-id="ac2b2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac2b2-134">Response</span></span>

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

