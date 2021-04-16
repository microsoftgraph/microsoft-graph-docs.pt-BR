---
title: Obter userExperienceAnalyticsDeviceScores
description: Leia propriedades e relações do objeto userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11114c40aa29de5c78283d065c30355a46fbea1f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868349"
---
# <a name="get-userexperienceanalyticsdevicescores"></a><span data-ttu-id="5cd89-103">Obter userExperienceAnalyticsDeviceScores</span><span class="sxs-lookup"><span data-stu-id="5cd89-103">Get userExperienceAnalyticsDeviceScores</span></span>

<span data-ttu-id="5cd89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cd89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cd89-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5cd89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cd89-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cd89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd89-107">Leia propriedades e relações do [objeto userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)</span><span class="sxs-lookup"><span data-stu-id="5cd89-107">Read properties and relationships of the [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cd89-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5cd89-108">Prerequisites</span></span>
<span data-ttu-id="5cd89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cd89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cd89-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cd89-111">Permission type</span></span>|<span data-ttu-id="5cd89-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5cd89-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cd89-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cd89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cd89-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd89-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5cd89-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cd89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cd89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cd89-116">Not supported.</span></span>|
|<span data-ttu-id="5cd89-117">Application</span><span class="sxs-lookup"><span data-stu-id="5cd89-117">Application</span></span>|<span data-ttu-id="5cd89-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd89-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cd89-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cd89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cd89-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5cd89-120">Optional query parameters</span></span>
<span data-ttu-id="5cd89-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5cd89-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cd89-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd89-122">Request headers</span></span>
|<span data-ttu-id="5cd89-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cd89-123">Header</span></span>|<span data-ttu-id="5cd89-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5cd89-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cd89-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cd89-125">Authorization</span></span>|<span data-ttu-id="5cd89-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cd89-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cd89-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5cd89-127">Accept</span></span>|<span data-ttu-id="5cd89-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5cd89-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cd89-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd89-129">Request body</span></span>
<span data-ttu-id="5cd89-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5cd89-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cd89-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cd89-131">Response</span></span>
<span data-ttu-id="5cd89-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cd89-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cd89-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cd89-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cd89-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cd89-134">Request</span></span>
<span data-ttu-id="5cd89-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cd89-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

### <a name="response"></a><span data-ttu-id="5cd89-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cd89-136">Response</span></span>
<span data-ttu-id="5cd89-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cd89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
    "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
    "deviceName": "Device Name value",
    "model": "Model value",
    "manufacturer": "Manufacturer value",
    "endpointAnalyticsScore": 7.333333333333333,
    "startupPerformanceScore": 7.666666666666667,
    "appReliabilityScore": 6.333333333333333
  }
}
```




