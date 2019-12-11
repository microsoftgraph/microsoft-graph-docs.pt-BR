---
title: Listar deviceHealthScriptDeviceStates
description: Listar Propriedades e relações dos objetos deviceHealthScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4ca756d773a504237338d16a63447a58a1509b6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945064"
---
# <a name="list-devicehealthscriptdevicestates"></a><span data-ttu-id="fc304-103">Listar deviceHealthScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="fc304-103">List deviceHealthScriptDeviceStates</span></span>

> <span data-ttu-id="fc304-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc304-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc304-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc304-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc304-106">Listar Propriedades e relações dos objetos [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="fc304-106">List properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc304-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc304-107">Prerequisites</span></span>
<span data-ttu-id="fc304-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc304-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc304-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc304-110">Permission type</span></span>|<span data-ttu-id="fc304-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc304-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc304-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc304-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc304-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc304-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fc304-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc304-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc304-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc304-115">Not supported.</span></span>|
|<span data-ttu-id="fc304-116">Application</span><span class="sxs-lookup"><span data-stu-id="fc304-116">Application</span></span>|<span data-ttu-id="fc304-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc304-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc304-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc304-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="fc304-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc304-119">Request headers</span></span>
|<span data-ttu-id="fc304-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc304-120">Header</span></span>|<span data-ttu-id="fc304-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fc304-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc304-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc304-122">Authorization</span></span>|<span data-ttu-id="fc304-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc304-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc304-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc304-124">Accept</span></span>|<span data-ttu-id="fc304-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc304-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc304-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc304-126">Request body</span></span>
<span data-ttu-id="fc304-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc304-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc304-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc304-128">Response</span></span>
<span data-ttu-id="fc304-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc304-129">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc304-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc304-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc304-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc304-131">Request</span></span>
<span data-ttu-id="fc304-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc304-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="fc304-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc304-133">Response</span></span>
<span data-ttu-id="fc304-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc304-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 892

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
      "id": "fd2e4505-4505-fd2e-0545-2efd05452efd",
      "detectionState": "success",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
      "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
      "remediationScriptError": "Remediation Script Error value",
      "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
      "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
      "remediationState": "skipped"
    }
  ]
}
```





