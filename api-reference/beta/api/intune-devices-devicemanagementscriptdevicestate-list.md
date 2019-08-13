---
title: Listar deviceManagementScriptDeviceStates
description: Listar Propriedades e relações dos objetos deviceManagementScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe14c5b2a866c36e50f097dd4c290823f56bf8ad
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310364"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="807ab-103">Listar deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="807ab-103">List deviceManagementScriptDeviceStates</span></span>

> <span data-ttu-id="807ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="807ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="807ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="807ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="807ab-106">Listar Propriedades e relações dos objetos [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="807ab-106">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="807ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="807ab-107">Prerequisites</span></span>
<span data-ttu-id="807ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="807ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="807ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="807ab-110">Permission type</span></span>|<span data-ttu-id="807ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="807ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="807ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="807ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="807ab-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="807ab-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="807ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="807ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="807ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="807ab-115">Not supported.</span></span>|
|<span data-ttu-id="807ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="807ab-116">Application</span></span>|<span data-ttu-id="807ab-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="807ab-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="807ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="807ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="807ab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="807ab-119">Request headers</span></span>
|<span data-ttu-id="807ab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="807ab-120">Header</span></span>|<span data-ttu-id="807ab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="807ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="807ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="807ab-122">Authorization</span></span>|<span data-ttu-id="807ab-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="807ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="807ab-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="807ab-124">Accept</span></span>|<span data-ttu-id="807ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="807ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="807ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="807ab-126">Request body</span></span>
<span data-ttu-id="807ab-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="807ab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="807ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="807ab-128">Response</span></span>
<span data-ttu-id="807ab-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="807ab-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="807ab-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="807ab-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="807ab-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="807ab-131">Request</span></span>
<span data-ttu-id="807ab-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="807ab-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="807ab-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="807ab-133">Response</span></span>
<span data-ttu-id="807ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="807ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
      "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
      "runState": "success",
      "resultMessage": "Result Message value",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
      "remediationScriptError": "Remediation Script Error value",
      "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value"
    }
  ]
}
```






