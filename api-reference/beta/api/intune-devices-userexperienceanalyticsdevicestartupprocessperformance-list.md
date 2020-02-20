---
title: Listar userExperienceAnalyticsDeviceStartupProcessPerformances
description: Listar Propriedades e relações dos objetos userExperienceAnalyticsDeviceStartupProcessPerformance.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d2a1dab1cbf5befc65d4cf7fe1bec457afcb681
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161949"
---
# <a name="list-userexperienceanalyticsdevicestartupprocessperformances"></a><span data-ttu-id="eb753-103">Listar userExperienceAnalyticsDeviceStartupProcessPerformances</span><span class="sxs-lookup"><span data-stu-id="eb753-103">List userExperienceAnalyticsDeviceStartupProcessPerformances</span></span>

> <span data-ttu-id="eb753-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb753-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb753-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb753-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb753-106">Listar Propriedades e relações dos objetos [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="eb753-106">List properties and relationships of the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb753-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb753-107">Prerequisites</span></span>
<span data-ttu-id="eb753-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb753-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb753-110">Permission type</span></span>|<span data-ttu-id="eb753-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb753-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb753-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb753-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb753-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb753-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="eb753-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb753-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb753-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb753-115">Not supported.</span></span>|
|<span data-ttu-id="eb753-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb753-116">Application</span></span>|<span data-ttu-id="eb753-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb753-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb753-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb753-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="eb753-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb753-119">Request headers</span></span>
|<span data-ttu-id="eb753-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb753-120">Header</span></span>|<span data-ttu-id="eb753-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb753-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb753-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb753-122">Authorization</span></span>|<span data-ttu-id="eb753-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb753-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb753-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb753-124">Accept</span></span>|<span data-ttu-id="eb753-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb753-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb753-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb753-126">Request body</span></span>
<span data-ttu-id="eb753-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb753-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb753-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb753-128">Response</span></span>
<span data-ttu-id="eb753-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb753-129">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb753-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb753-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb753-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb753-131">Request</span></span>
<span data-ttu-id="eb753-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb753-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

### <a name="response"></a><span data-ttu-id="eb753-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb753-133">Response</span></span>
<span data-ttu-id="eb753-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb753-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





