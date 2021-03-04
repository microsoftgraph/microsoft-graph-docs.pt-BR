---
title: função summarizeDeviceRemoteConnection
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23053d4e61ad3f60fc2a4a7d8090d5c692d2f0eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445698"
---
# <a name="summarizedeviceremoteconnection-function"></a><span data-ttu-id="40942-103">função summarizeDeviceRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="40942-103">summarizeDeviceRemoteConnection function</span></span>

<span data-ttu-id="40942-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40942-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40942-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40942-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40942-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40942-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40942-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="40942-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40942-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40942-108">Prerequisites</span></span>
<span data-ttu-id="40942-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40942-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40942-111">Permission type</span></span>|<span data-ttu-id="40942-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40942-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40942-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40942-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40942-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40942-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40942-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40942-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40942-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40942-116">Not supported.</span></span>|
|<span data-ttu-id="40942-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40942-117">Application</span></span>|<span data-ttu-id="40942-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40942-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40942-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40942-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRemoteConnection/summarizeDeviceRemoteConnection
```

## <a name="request-headers"></a><span data-ttu-id="40942-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40942-120">Request headers</span></span>
|<span data-ttu-id="40942-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40942-121">Header</span></span>|<span data-ttu-id="40942-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40942-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40942-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40942-123">Authorization</span></span>|<span data-ttu-id="40942-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40942-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40942-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40942-125">Accept</span></span>|<span data-ttu-id="40942-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40942-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40942-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40942-127">Request body</span></span>
<span data-ttu-id="40942-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="40942-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="40942-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="40942-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="40942-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40942-130">Property</span></span>|<span data-ttu-id="40942-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="40942-131">Type</span></span>|<span data-ttu-id="40942-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="40942-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40942-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="40942-133">summarizeBy</span></span>|[<span data-ttu-id="40942-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="40942-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="40942-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="40942-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="40942-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="40942-136">Response</span></span>
<span data-ttu-id="40942-137">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40942-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40942-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40942-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="40942-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40942-139">Request</span></span>
<span data-ttu-id="40942-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40942-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/summarizeDeviceRemoteConnection(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="40942-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="40942-141">Response</span></span>
<span data-ttu-id="40942-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40942-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
      "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "model": "Model value",
      "virtualNetwork": "Virtual Network value",
      "deviceCount": 11,
      "cloudPcRoundTripTime": 6.666666666666667,
      "cloudPcSignInTime": 5.666666666666667,
      "remoteSignInTime": 5.333333333333333,
      "coreBootTime": 4.0,
      "coreSignInTime": 4.666666666666667,
      "cloudPcFailurePercentage": 8.0
    }
  ]
}
```




