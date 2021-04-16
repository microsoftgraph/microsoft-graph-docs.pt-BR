---
title: Listar userExperienceAnalyticsDeviceScoreses
description: Listar propriedades e relações dos objetos userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38dd723dde8ae420967e46350caec0708d5e1e92
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868348"
---
# <a name="list-userexperienceanalyticsdevicescoreses"></a><span data-ttu-id="c59a8-103">Listar userExperienceAnalyticsDeviceScoreses</span><span class="sxs-lookup"><span data-stu-id="c59a8-103">List userExperienceAnalyticsDeviceScoreses</span></span>

<span data-ttu-id="c59a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c59a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c59a8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c59a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c59a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c59a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c59a8-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)</span><span class="sxs-lookup"><span data-stu-id="c59a8-107">List properties and relationships of the [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c59a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c59a8-108">Prerequisites</span></span>
<span data-ttu-id="c59a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c59a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c59a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c59a8-111">Permission type</span></span>|<span data-ttu-id="c59a8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c59a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c59a8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c59a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c59a8-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c59a8-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c59a8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c59a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c59a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c59a8-116">Not supported.</span></span>|
|<span data-ttu-id="c59a8-117">Application</span><span class="sxs-lookup"><span data-stu-id="c59a8-117">Application</span></span>|<span data-ttu-id="c59a8-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c59a8-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c59a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c59a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceScores
```

## <a name="request-headers"></a><span data-ttu-id="c59a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c59a8-120">Request headers</span></span>
|<span data-ttu-id="c59a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c59a8-121">Header</span></span>|<span data-ttu-id="c59a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c59a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c59a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c59a8-123">Authorization</span></span>|<span data-ttu-id="c59a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c59a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c59a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c59a8-125">Accept</span></span>|<span data-ttu-id="c59a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c59a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c59a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c59a8-127">Request body</span></span>
<span data-ttu-id="c59a8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c59a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c59a8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c59a8-129">Response</span></span>
<span data-ttu-id="c59a8-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c59a8-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c59a8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c59a8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c59a8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c59a8-132">Request</span></span>
<span data-ttu-id="c59a8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c59a8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores
```

### <a name="response"></a><span data-ttu-id="c59a8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c59a8-134">Response</span></span>
<span data-ttu-id="c59a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c59a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
      "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
      "deviceName": "Device Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "endpointAnalyticsScore": 7.333333333333333,
      "startupPerformanceScore": 7.666666666666667,
      "appReliabilityScore": 6.333333333333333
    }
  ]
}
```




