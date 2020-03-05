---
title: Listar userExperienceAnalyticsDeviceStartupProcessPerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsDeviceStartupProcessPerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ed9001fbbc7be6956e048004b1e38a05ef1ea79
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468254"
---
# <a name="list-userexperienceanalyticsdevicestartupprocessperformances"></a><span data-ttu-id="5abdd-103">Listar userExperienceAnalyticsDeviceStartupProcessPerformances</span><span class="sxs-lookup"><span data-stu-id="5abdd-103">List userExperienceAnalyticsDeviceStartupProcessPerformances</span></span>

<span data-ttu-id="5abdd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5abdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5abdd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5abdd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5abdd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5abdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5abdd-107">Listar Propriedades e relações dos objetos [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="5abdd-107">List properties and relationships of the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5abdd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5abdd-108">Prerequisites</span></span>
<span data-ttu-id="5abdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5abdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5abdd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5abdd-111">Permission type</span></span>|<span data-ttu-id="5abdd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5abdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5abdd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5abdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5abdd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5abdd-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5abdd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5abdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5abdd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5abdd-116">Not supported.</span></span>|
|<span data-ttu-id="5abdd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5abdd-117">Application</span></span>|<span data-ttu-id="5abdd-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5abdd-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5abdd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5abdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="5abdd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5abdd-120">Request headers</span></span>
|<span data-ttu-id="5abdd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5abdd-121">Header</span></span>|<span data-ttu-id="5abdd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5abdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5abdd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5abdd-123">Authorization</span></span>|<span data-ttu-id="5abdd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5abdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5abdd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5abdd-125">Accept</span></span>|<span data-ttu-id="5abdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5abdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5abdd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5abdd-127">Request body</span></span>
<span data-ttu-id="5abdd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5abdd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5abdd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5abdd-129">Response</span></span>
<span data-ttu-id="5abdd-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5abdd-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5abdd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5abdd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5abdd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5abdd-132">Request</span></span>
<span data-ttu-id="5abdd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5abdd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

### <a name="response"></a><span data-ttu-id="5abdd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5abdd-134">Response</span></span>
<span data-ttu-id="5abdd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5abdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
      "id": "86c4355c-355c-86c4-5c35-c4865c35c486",
      "processName": "Process Name value",
      "productName": "Product Name value",
      "publisher": "Publisher value",
      "deviceCount": 11,
      "medianImpactInMs": 0,
      "totalImpactInMs": 15
    }
  ]
}
```





