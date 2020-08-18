---
title: Obter userExperienceAnalyticsDeviceStartupHistory
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93fa666edfadc398c5809644cd656f78923aa063
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791355"
---
# <a name="get-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="675d7-103">Obter userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="675d7-103">Get userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="675d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="675d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="675d7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="675d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="675d7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="675d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="675d7-107">Leia as propriedades e as relações do objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="675d7-107">Read properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="675d7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="675d7-108">Prerequisites</span></span>
<span data-ttu-id="675d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="675d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="675d7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="675d7-111">Permission type</span></span>|<span data-ttu-id="675d7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="675d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="675d7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="675d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="675d7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="675d7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="675d7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="675d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="675d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="675d7-116">Not supported.</span></span>|
|<span data-ttu-id="675d7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="675d7-117">Application</span></span>|<span data-ttu-id="675d7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="675d7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="675d7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="675d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="675d7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="675d7-120">Optional query parameters</span></span>
<span data-ttu-id="675d7-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="675d7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="675d7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="675d7-122">Request headers</span></span>
|<span data-ttu-id="675d7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="675d7-123">Header</span></span>|<span data-ttu-id="675d7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="675d7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="675d7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="675d7-125">Authorization</span></span>|<span data-ttu-id="675d7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="675d7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="675d7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="675d7-127">Accept</span></span>|<span data-ttu-id="675d7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="675d7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="675d7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="675d7-129">Request body</span></span>
<span data-ttu-id="675d7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="675d7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="675d7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="675d7-131">Response</span></span>
<span data-ttu-id="675d7-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="675d7-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="675d7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="675d7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="675d7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="675d7-134">Request</span></span>
<span data-ttu-id="675d7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="675d7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

### <a name="response"></a><span data-ttu-id="675d7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="675d7-136">Response</span></span>
<span data-ttu-id="675d7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="675d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 676

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
    "restartCategory": "restartWithUpdate"
  }
}
```



