---
title: Obter deviceManagementScriptDeviceState
description: Leia as propriedades e as relações do objeto deviceManagementScriptDeviceState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c1b77d65fcbfa85d44dfe2919347efd8ad74bb9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814446"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="06e00-103">Obter deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="06e00-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="06e00-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06e00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06e00-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06e00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06e00-106">Leia as propriedades e as relações do objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="06e00-106">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06e00-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06e00-107">Prerequisites</span></span>
<span data-ttu-id="06e00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06e00-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06e00-110">Permission type</span></span>|<span data-ttu-id="06e00-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06e00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06e00-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06e00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06e00-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="06e00-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="06e00-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06e00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06e00-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06e00-115">Not supported.</span></span>|
|<span data-ttu-id="06e00-116">Application</span><span class="sxs-lookup"><span data-stu-id="06e00-116">Application</span></span>|<span data-ttu-id="06e00-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="06e00-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06e00-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06e00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06e00-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="06e00-119">Optional query parameters</span></span>
<span data-ttu-id="06e00-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="06e00-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06e00-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06e00-121">Request headers</span></span>
|<span data-ttu-id="06e00-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06e00-122">Header</span></span>|<span data-ttu-id="06e00-123">Valor</span><span class="sxs-lookup"><span data-stu-id="06e00-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06e00-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="06e00-124">Authorization</span></span>|<span data-ttu-id="06e00-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06e00-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06e00-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06e00-126">Accept</span></span>|<span data-ttu-id="06e00-127">application/json</span><span class="sxs-lookup"><span data-stu-id="06e00-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06e00-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06e00-128">Request body</span></span>
<span data-ttu-id="06e00-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06e00-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06e00-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="06e00-130">Response</span></span>
<span data-ttu-id="06e00-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06e00-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06e00-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06e00-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="06e00-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06e00-133">Request</span></span>
<span data-ttu-id="06e00-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06e00-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="06e00-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="06e00-135">Response</span></span>
<span data-ttu-id="06e00-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06e00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




