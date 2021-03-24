---
title: ação getAssignmentFiltersStatusDetails
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2538cc410dbe3b80ea1b2e26c5fe3c4c9bedafca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148670"
---
# <a name="getassignmentfiltersstatusdetails-action"></a><span data-ttu-id="c9f23-103">ação getAssignmentFiltersStatusDetails</span><span class="sxs-lookup"><span data-stu-id="c9f23-103">getAssignmentFiltersStatusDetails action</span></span>

<span data-ttu-id="c9f23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9f23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9f23-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9f23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9f23-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9f23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9f23-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9f23-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9f23-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9f23-108">Prerequisites</span></span>
<span data-ttu-id="c9f23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9f23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9f23-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9f23-111">Permission type</span></span>|<span data-ttu-id="c9f23-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9f23-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9f23-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9f23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9f23-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9f23-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9f23-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9f23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9f23-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9f23-116">Not supported.</span></span>|
|<span data-ttu-id="c9f23-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9f23-117">Application</span></span>|<span data-ttu-id="c9f23-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9f23-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9f23-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9f23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/getAssignmentFiltersStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="c9f23-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f23-120">Request headers</span></span>
|<span data-ttu-id="c9f23-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9f23-121">Header</span></span>|<span data-ttu-id="c9f23-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c9f23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9f23-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9f23-123">Authorization</span></span>|<span data-ttu-id="c9f23-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9f23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9f23-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9f23-125">Accept</span></span>|<span data-ttu-id="c9f23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9f23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9f23-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f23-127">Request body</span></span>
<span data-ttu-id="c9f23-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c9f23-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c9f23-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c9f23-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c9f23-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9f23-130">Property</span></span>|<span data-ttu-id="c9f23-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9f23-131">Type</span></span>|<span data-ttu-id="c9f23-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9f23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9f23-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c9f23-133">managedDeviceId</span></span>|<span data-ttu-id="c9f23-134">String</span><span class="sxs-lookup"><span data-stu-id="c9f23-134">String</span></span>|<span data-ttu-id="c9f23-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9f23-135">Not yet documented</span></span>|
|<span data-ttu-id="c9f23-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="c9f23-136">payloadId</span></span>|<span data-ttu-id="c9f23-137">String</span><span class="sxs-lookup"><span data-stu-id="c9f23-137">String</span></span>|<span data-ttu-id="c9f23-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9f23-138">Not yet documented</span></span>|
|<span data-ttu-id="c9f23-139">userId</span><span class="sxs-lookup"><span data-stu-id="c9f23-139">userId</span></span>|<span data-ttu-id="c9f23-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9f23-140">String</span></span>|<span data-ttu-id="c9f23-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9f23-141">Not yet documented</span></span>|
|<span data-ttu-id="c9f23-142">assignmentFilterIds</span><span class="sxs-lookup"><span data-stu-id="c9f23-142">assignmentFilterIds</span></span>|<span data-ttu-id="c9f23-143">String collection</span><span class="sxs-lookup"><span data-stu-id="c9f23-143">String collection</span></span>|<span data-ttu-id="c9f23-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9f23-144">Not yet documented</span></span>|
|<span data-ttu-id="c9f23-145">top</span><span class="sxs-lookup"><span data-stu-id="c9f23-145">top</span></span>|<span data-ttu-id="c9f23-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c9f23-146">Int32</span></span>|<span data-ttu-id="c9f23-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9f23-147">Not yet documented</span></span>|
|<span data-ttu-id="c9f23-148">skip</span><span class="sxs-lookup"><span data-stu-id="c9f23-148">skip</span></span>|<span data-ttu-id="c9f23-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c9f23-149">Int32</span></span>|<span data-ttu-id="c9f23-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c9f23-150">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c9f23-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9f23-151">Response</span></span>
<span data-ttu-id="c9f23-152">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [assignmentFilterStatusDetails](../resources/intune-policyset-assignmentfilterstatusdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9f23-152">If successful, this action returns a `200 OK` response code and a [assignmentFilterStatusDetails](../resources/intune-policyset-assignmentfilterstatusdetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9f23-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9f23-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9f23-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f23-154">Request</span></span>
<span data-ttu-id="c9f23-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9f23-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9f23-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9f23-156">Response</span></span>
<span data-ttu-id="c9f23-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9f23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

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
        "assignmentFilterType": "include",
        "assignmentFilterTypeAndEvaluationResults": [
          {
            "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
            "assignmentFilterType": "include",
            "evaluationResult": "match"
          }
        ]
      }
    ]
  }
}
```




