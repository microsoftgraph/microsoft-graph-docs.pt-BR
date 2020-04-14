---
title: ação getDevicesScheduledToRetire
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 006f71353658fcbc0d8deffc3283fe861877b9aa
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434121"
---
# <a name="getdevicesscheduledtoretire-action"></a><span data-ttu-id="1f1c4-103">ação getDevicesScheduledToRetire</span><span class="sxs-lookup"><span data-stu-id="1f1c4-103">getDevicesScheduledToRetire action</span></span>

<span data-ttu-id="1f1c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f1c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f1c4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f1c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f1c4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f1c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f1c4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1f1c4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f1c4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f1c4-108">Prerequisites</span></span>
<span data-ttu-id="1f1c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f1c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f1c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f1c4-111">Permission type</span></span>|<span data-ttu-id="1f1c4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1f1c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f1c4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f1c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f1c4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f1c4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1f1c4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f1c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f1c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f1c4-116">Not supported.</span></span>|
|<span data-ttu-id="1f1c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f1c4-117">Application</span></span>|<span data-ttu-id="1f1c4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f1c4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f1c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f1c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

## <a name="request-headers"></a><span data-ttu-id="1f1c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f1c4-120">Request headers</span></span>
|<span data-ttu-id="1f1c4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f1c4-121">Header</span></span>|<span data-ttu-id="1f1c4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1f1c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f1c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f1c4-123">Authorization</span></span>|<span data-ttu-id="1f1c4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f1c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f1c4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f1c4-125">Accept</span></span>|<span data-ttu-id="1f1c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f1c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f1c4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f1c4-127">Request body</span></span>
<span data-ttu-id="1f1c4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f1c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f1c4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f1c4-129">Response</span></span>
<span data-ttu-id="1f1c4-130">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [retireScheduledManagedDevice](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f1c4-130">If successful, this action returns a `200 OK` response code and a [retireScheduledManagedDevice](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f1c4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f1c4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f1c4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f1c4-132">Request</span></span>
<span data-ttu-id="1f1c4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f1c4-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

### <a name="response"></a><span data-ttu-id="1f1c4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f1c4-134">Response</span></span>
<span data-ttu-id="1f1c4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f1c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 596

{
  "value": [
    {
      "@odata.type": "microsoft.graph.retireScheduledManagedDevice",
      "id": "Id value",
      "managedDeviceId": "Managed Device Id value",
      "managedDeviceName": "Managed Device Name value",
      "deviceType": "windowsRT",
      "complianceState": "notApplicable",
      "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
      "managementAgent": "mdm",
      "ownerType": "company",
      "deviceCompliancePolicyName": "Device Compliance Policy Name value",
      "deviceCompliancePolicyId": "Device Compliance Policy Id value"
    }
  ]
}
```



