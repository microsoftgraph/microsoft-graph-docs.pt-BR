---
title: Obter deviceHealthScriptDeviceState
description: Leia as propriedades e as relações do objeto deviceHealthScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e360630e3d74d80df03a0d30652272c71ab330c7
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162124"
---
# <a name="get-devicehealthscriptdevicestate"></a><span data-ttu-id="e5332-103">Obter deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="e5332-103">Get deviceHealthScriptDeviceState</span></span>

> <span data-ttu-id="e5332-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5332-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5332-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5332-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5332-106">Leia as propriedades e as relações do objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e5332-106">Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5332-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5332-107">Prerequisites</span></span>
<span data-ttu-id="e5332-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5332-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5332-110">Permission type</span></span>|<span data-ttu-id="e5332-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5332-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5332-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5332-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5332-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5332-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e5332-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5332-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5332-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5332-115">Not supported.</span></span>|
|<span data-ttu-id="e5332-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5332-116">Application</span></span>|<span data-ttu-id="e5332-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5332-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5332-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5332-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5332-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e5332-119">Optional query parameters</span></span>
<span data-ttu-id="e5332-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e5332-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5332-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5332-121">Request headers</span></span>
|<span data-ttu-id="e5332-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5332-122">Header</span></span>|<span data-ttu-id="e5332-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e5332-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5332-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5332-124">Authorization</span></span>|<span data-ttu-id="e5332-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5332-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5332-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5332-126">Accept</span></span>|<span data-ttu-id="e5332-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e5332-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5332-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5332-128">Request body</span></span>
<span data-ttu-id="e5332-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5332-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5332-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5332-130">Response</span></span>
<span data-ttu-id="e5332-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5332-131">If successful, this method returns a `200 OK` response code and [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5332-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5332-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5332-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5332-133">Request</span></span>
<span data-ttu-id="e5332-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5332-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="e5332-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5332-135">Response</span></span>
<span data-ttu-id="e5332-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5332-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "value": {
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
}
```





