---
title: Obter userExperienceAnalyticsDeviceStartupHistory
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2934247c34ce80078f19685dd7c547a664f6470e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234311"
---
# <a name="get-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="83d91-103">Obter userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="83d91-103">Get userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="83d91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83d91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83d91-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83d91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83d91-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83d91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83d91-107">Leia as propriedades e as relações do objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="83d91-107">Read properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83d91-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83d91-108">Prerequisites</span></span>
<span data-ttu-id="83d91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83d91-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83d91-111">Permission type</span></span>|<span data-ttu-id="83d91-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83d91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83d91-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83d91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83d91-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="83d91-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="83d91-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83d91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83d91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83d91-116">Not supported.</span></span>|
|<span data-ttu-id="83d91-117">Application</span><span class="sxs-lookup"><span data-stu-id="83d91-117">Application</span></span>|<span data-ttu-id="83d91-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="83d91-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83d91-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83d91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83d91-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83d91-120">Optional query parameters</span></span>
<span data-ttu-id="83d91-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83d91-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83d91-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83d91-122">Request headers</span></span>
|<span data-ttu-id="83d91-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83d91-123">Header</span></span>|<span data-ttu-id="83d91-124">Valor</span><span class="sxs-lookup"><span data-stu-id="83d91-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83d91-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="83d91-125">Authorization</span></span>|<span data-ttu-id="83d91-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83d91-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83d91-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83d91-127">Accept</span></span>|<span data-ttu-id="83d91-128">application/json</span><span class="sxs-lookup"><span data-stu-id="83d91-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83d91-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83d91-129">Request body</span></span>
<span data-ttu-id="83d91-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83d91-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83d91-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d91-131">Response</span></span>
<span data-ttu-id="83d91-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83d91-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83d91-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83d91-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="83d91-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83d91-134">Request</span></span>
<span data-ttu-id="83d91-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83d91-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

### <a name="response"></a><span data-ttu-id="83d91-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d91-136">Response</span></span>
<span data-ttu-id="83d91-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83d91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 784

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
    "id": "13357123-7123-1335-2371-351323713513",
    "deviceId": "Device Id value",
    "startTime": "2017-01-01T00:03:29.2730865-08:00",
    "coreBootTimeInMs": 0,
    "groupPolicyBootTimeInMs": 7,
    "featureUpdateBootTimeInMs": 9,
    "totalBootTimeInMs": 1,
    "groupPolicyLoginTimeInMs": 8,
    "coreLoginTimeInMs": 1,
    "responsiveDesktopTimeInMs": 9,
    "totalLoginTimeInMs": 2,
    "isFirstLogin": true,
    "isFeatureUpdate": true,
    "operatingSystemVersion": "Operating System Version value",
    "restartCategory": "restartWithUpdate",
    "restartStopCode": "Restart Stop Code value",
    "restartFaultBucket": "Restart Fault Bucket value"
  }
}
```




