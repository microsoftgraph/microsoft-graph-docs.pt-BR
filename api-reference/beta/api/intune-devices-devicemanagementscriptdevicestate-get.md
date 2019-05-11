---
title: Obter deviceManagementScriptDeviceState
description: Leia as propriedades e as relações do objeto deviceManagementScriptDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba27d543e7eaa7632dc716ffe8ea65feb2806b60
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909866"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="d57ca-103">Obter deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="d57ca-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="d57ca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d57ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d57ca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d57ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d57ca-106">Leia as propriedades e as relações do objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d57ca-106">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d57ca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d57ca-107">Prerequisites</span></span>
<span data-ttu-id="d57ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d57ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d57ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d57ca-110">Permission type</span></span>|<span data-ttu-id="d57ca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d57ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d57ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d57ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d57ca-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d57ca-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d57ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d57ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d57ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d57ca-115">Not supported.</span></span>|
|<span data-ttu-id="d57ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d57ca-116">Application</span></span>|<span data-ttu-id="d57ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d57ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d57ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d57ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d57ca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d57ca-119">Optional query parameters</span></span>
<span data-ttu-id="d57ca-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d57ca-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d57ca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d57ca-121">Request headers</span></span>
|<span data-ttu-id="d57ca-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d57ca-122">Header</span></span>|<span data-ttu-id="d57ca-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d57ca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d57ca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d57ca-124">Authorization</span></span>|<span data-ttu-id="d57ca-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d57ca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d57ca-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d57ca-126">Accept</span></span>|<span data-ttu-id="d57ca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d57ca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d57ca-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d57ca-128">Request body</span></span>
<span data-ttu-id="d57ca-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d57ca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d57ca-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d57ca-130">Response</span></span>
<span data-ttu-id="d57ca-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d57ca-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d57ca-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d57ca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d57ca-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d57ca-133">Request</span></span>
<span data-ttu-id="d57ca-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d57ca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="d57ca-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d57ca-135">Response</span></span>
<span data-ttu-id="d57ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d57ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
    "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
    "runState": "success",
    "resultMessage": "Result Message value",
    "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
    "errorCode": 9,
    "errorDescription": "Error Description value"
  }
}
```




