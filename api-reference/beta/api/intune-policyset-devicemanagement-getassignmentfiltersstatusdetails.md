---
title: Ação getAssignmentFiltersStatusDetails
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40bcb746bc4997c2cb0742dd2ef66ff1f84a0634
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160094"
---
# <a name="getassignmentfiltersstatusdetails-action"></a><span data-ttu-id="b079c-103">Ação getAssignmentFiltersStatusDetails</span><span class="sxs-lookup"><span data-stu-id="b079c-103">getAssignmentFiltersStatusDetails action</span></span>

<span data-ttu-id="b079c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b079c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b079c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b079c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b079c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b079c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b079c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b079c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b079c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b079c-108">Prerequisites</span></span>
<span data-ttu-id="b079c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b079c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b079c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b079c-111">Permission type</span></span>|<span data-ttu-id="b079c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b079c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b079c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b079c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b079c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b079c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b079c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b079c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b079c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b079c-116">Not supported.</span></span>|
|<span data-ttu-id="b079c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b079c-117">Application</span></span>|<span data-ttu-id="b079c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b079c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b079c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b079c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/getAssignmentFiltersStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="b079c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b079c-120">Request headers</span></span>
|<span data-ttu-id="b079c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b079c-121">Header</span></span>|<span data-ttu-id="b079c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b079c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b079c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b079c-123">Authorization</span></span>|<span data-ttu-id="b079c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b079c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b079c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b079c-125">Accept</span></span>|<span data-ttu-id="b079c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b079c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b079c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b079c-127">Request body</span></span>
<span data-ttu-id="b079c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b079c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b079c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b079c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b079c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b079c-130">Property</span></span>|<span data-ttu-id="b079c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b079c-131">Type</span></span>|<span data-ttu-id="b079c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b079c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b079c-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b079c-133">managedDeviceId</span></span>|<span data-ttu-id="b079c-134">String</span><span class="sxs-lookup"><span data-stu-id="b079c-134">String</span></span>|<span data-ttu-id="b079c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b079c-135">Not yet documented</span></span>|
|<span data-ttu-id="b079c-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="b079c-136">payloadId</span></span>|<span data-ttu-id="b079c-137">String</span><span class="sxs-lookup"><span data-stu-id="b079c-137">String</span></span>|<span data-ttu-id="b079c-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b079c-138">Not yet documented</span></span>|
|<span data-ttu-id="b079c-139">userId</span><span class="sxs-lookup"><span data-stu-id="b079c-139">userId</span></span>|<span data-ttu-id="b079c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b079c-140">String</span></span>|<span data-ttu-id="b079c-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b079c-141">Not yet documented</span></span>|
|<span data-ttu-id="b079c-142">assignmentFilterIds</span><span class="sxs-lookup"><span data-stu-id="b079c-142">assignmentFilterIds</span></span>|<span data-ttu-id="b079c-143">String collection</span><span class="sxs-lookup"><span data-stu-id="b079c-143">String collection</span></span>|<span data-ttu-id="b079c-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b079c-144">Not yet documented</span></span>|
|<span data-ttu-id="b079c-145">top</span><span class="sxs-lookup"><span data-stu-id="b079c-145">top</span></span>|<span data-ttu-id="b079c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b079c-146">Int32</span></span>|<span data-ttu-id="b079c-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b079c-147">Not yet documented</span></span>|
|<span data-ttu-id="b079c-148">skip</span><span class="sxs-lookup"><span data-stu-id="b079c-148">skip</span></span>|<span data-ttu-id="b079c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b079c-149">Int32</span></span>|<span data-ttu-id="b079c-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b079c-150">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b079c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b079c-151">Response</span></span>
<span data-ttu-id="b079c-152">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um [assignmentFilterStatusDetails](../resources/intune-policyset-assignmentfilterstatusdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b079c-152">If successful, this action returns a `200 OK` response code and a [assignmentFilterStatusDetails](../resources/intune-policyset-assignmentfilterstatusdetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b079c-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b079c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="b079c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b079c-154">Request</span></span>
<span data-ttu-id="b079c-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b079c-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/getAssignmentFiltersStatusDetails

Content-type: application/json
Content-length: 214

{
  "managedDeviceId": "Managed Device Id value",
  "payloadId": "Payload Id value",
  "userId": "User Id value",
  "assignmentFilterIds": [
    "Assignment Filter Ids value"
  ],
  "top": 3,
  "skip": 4
}
```

### <a name="response"></a><span data-ttu-id="b079c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b079c-156">Response</span></span>
<span data-ttu-id="b079c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b079c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 947

{
  "value": {
    "@odata.type": "microsoft.graph.assignmentFilterStatusDetails",
    "managedDeviceId": "Managed Device Id value",
    "payloadId": "Payload Id value",
    "userId": "User Id value",
    "deviceProperties": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "evalutionSummaries": [
      {
        "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
        "assignmentFilterId": "Assignment Filter Id value",
        "assignmentFilterLastModifiedDateTime": "2017-01-01T00:02:50.0900701-08:00",
        "assignmentFilterDisplayName": "Assignment Filter Display Name value",
        "assignmentFilterPlatform": "androidForWork",
        "evaluationResult": "match",
        "evaluationDateTime": "2016-12-31T23:58:01.2047675-08:00",
        "assignmentFilterType": "include"
      }
    ]
  }
}
```




