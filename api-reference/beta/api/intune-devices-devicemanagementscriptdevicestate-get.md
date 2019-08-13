---
title: Obter deviceManagementScriptDeviceState
description: Leia as propriedades e as relações do objeto deviceManagementScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e75c913fc0972f16a08807af71d24a3fd02a1e65
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310357"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="0e570-103">Obter deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0e570-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="0e570-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e570-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e570-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e570-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e570-106">Leia as propriedades e as relações do objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="0e570-106">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e570-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e570-107">Prerequisites</span></span>
<span data-ttu-id="0e570-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e570-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e570-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e570-110">Permission type</span></span>|<span data-ttu-id="0e570-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0e570-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e570-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e570-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e570-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e570-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0e570-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e570-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e570-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e570-115">Not supported.</span></span>|
|<span data-ttu-id="0e570-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e570-116">Application</span></span>|<span data-ttu-id="0e570-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e570-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e570-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e570-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e570-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e570-119">Optional query parameters</span></span>
<span data-ttu-id="0e570-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e570-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e570-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e570-121">Request headers</span></span>
|<span data-ttu-id="0e570-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e570-122">Header</span></span>|<span data-ttu-id="0e570-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0e570-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e570-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e570-124">Authorization</span></span>|<span data-ttu-id="0e570-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e570-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e570-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e570-126">Accept</span></span>|<span data-ttu-id="0e570-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0e570-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e570-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e570-128">Request body</span></span>
<span data-ttu-id="0e570-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e570-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e570-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e570-130">Response</span></span>
<span data-ttu-id="0e570-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e570-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e570-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e570-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e570-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e570-133">Request</span></span>
<span data-ttu-id="0e570-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e570-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="0e570-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e570-135">Response</span></span>
<span data-ttu-id="0e570-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e570-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 678

{
  "value": {
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
}
```






