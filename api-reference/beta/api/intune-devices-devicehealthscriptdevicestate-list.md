---
title: Listar deviceHealthScriptDeviceStates
description: Listar propriedades e relações dos objetos deviceHealthScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0539b09d96e43bde2ff099b89fcec81c4c5e2ae4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665305"
---
# <a name="list-devicehealthscriptdevicestates"></a><span data-ttu-id="7a1aa-103">Listar deviceHealthScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="7a1aa-103">List deviceHealthScriptDeviceStates</span></span>

<span data-ttu-id="7a1aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a1aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a1aa-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a1aa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a1aa-107">Listar propriedades e relações dos [objetos deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="7a1aa-107">List properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a1aa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a1aa-108">Prerequisites</span></span>
<span data-ttu-id="7a1aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a1aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a1aa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a1aa-111">Permission type</span></span>|<span data-ttu-id="7a1aa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a1aa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a1aa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a1aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a1aa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a1aa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a1aa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a1aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a1aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-116">Not supported.</span></span>|
|<span data-ttu-id="7a1aa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a1aa-117">Application</span></span>|<span data-ttu-id="7a1aa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a1aa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a1aa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a1aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="7a1aa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a1aa-120">Request headers</span></span>
|<span data-ttu-id="7a1aa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a1aa-121">Header</span></span>|<span data-ttu-id="7a1aa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7a1aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a1aa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a1aa-123">Authorization</span></span>|<span data-ttu-id="7a1aa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a1aa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a1aa-125">Accept</span></span>|<span data-ttu-id="7a1aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a1aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a1aa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a1aa-127">Request body</span></span>
<span data-ttu-id="7a1aa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a1aa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a1aa-129">Response</span></span>
<span data-ttu-id="7a1aa-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-130">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a1aa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a1aa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a1aa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a1aa-132">Request</span></span>
<span data-ttu-id="7a1aa-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="7a1aa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a1aa-134">Response</span></span>
<span data-ttu-id="7a1aa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a1aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 973

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
      "remediationState": "skipped",
      "assignmentFilterIds": [
        "Assignment Filter Ids value"
      ]
    }
  ]
}
```




