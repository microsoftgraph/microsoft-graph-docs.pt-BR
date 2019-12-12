---
title: ação getDevicesScheduledToRetire
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f70d3e01838de20b890eed12b8b92d0171bf0c85
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949711"
---
# <a name="getdevicesscheduledtoretire-action"></a><span data-ttu-id="eb781-103">ação getDevicesScheduledToRetire</span><span class="sxs-lookup"><span data-stu-id="eb781-103">getDevicesScheduledToRetire action</span></span>

> <span data-ttu-id="eb781-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb781-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb781-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb781-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb781-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eb781-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb781-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb781-107">Prerequisites</span></span>
<span data-ttu-id="eb781-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb781-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb781-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb781-110">Permission type</span></span>|<span data-ttu-id="eb781-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb781-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb781-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb781-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb781-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb781-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eb781-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb781-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb781-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb781-115">Not supported.</span></span>|
|<span data-ttu-id="eb781-116">Application</span><span class="sxs-lookup"><span data-stu-id="eb781-116">Application</span></span>|<span data-ttu-id="eb781-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb781-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb781-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb781-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

## <a name="request-headers"></a><span data-ttu-id="eb781-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb781-119">Request headers</span></span>
|<span data-ttu-id="eb781-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb781-120">Header</span></span>|<span data-ttu-id="eb781-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb781-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb781-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb781-122">Authorization</span></span>|<span data-ttu-id="eb781-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb781-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb781-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb781-124">Accept</span></span>|<span data-ttu-id="eb781-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb781-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb781-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb781-126">Request body</span></span>
<span data-ttu-id="eb781-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb781-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb781-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb781-128">Response</span></span>
<span data-ttu-id="eb781-129">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [retireScheduledManagedDevice](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb781-129">If successful, this action returns a `200 OK` response code and a [retireScheduledManagedDevice](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb781-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb781-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb781-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb781-131">Request</span></span>
<span data-ttu-id="eb781-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb781-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

### <a name="response"></a><span data-ttu-id="eb781-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb781-133">Response</span></span>
<span data-ttu-id="eb781-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb781-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





