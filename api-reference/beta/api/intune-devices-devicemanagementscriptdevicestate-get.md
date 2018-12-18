---
title: Obter deviceManagementScriptDeviceState
description: Leia as propriedades e os relacionamentos do objeto deviceManagementScriptDeviceState.
author: tfitzmac
ms.openlocfilehash: 4a050737c4e4aedd9c42228fc685ebfeb3bc02f2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349753"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="7fe77-103">Obter deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="7fe77-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="7fe77-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7fe77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fe77-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7fe77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fe77-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7fe77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fe77-107">Leia as propriedades e os relacionamentos do objeto [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="7fe77-107">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fe77-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7fe77-108">Prerequisites</span></span>
<span data-ttu-id="7fe77-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fe77-111">Permission type</span></span>|<span data-ttu-id="7fe77-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7fe77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fe77-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fe77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fe77-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fe77-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7fe77-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fe77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fe77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe77-116">Not supported.</span></span>|
|<span data-ttu-id="7fe77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fe77-117">Application</span></span>|<span data-ttu-id="7fe77-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe77-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fe77-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7fe77-120">Optional query parameters</span></span>
<span data-ttu-id="7fe77-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe77-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7fe77-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe77-122">Request headers</span></span>
|<span data-ttu-id="7fe77-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fe77-123">Header</span></span>|<span data-ttu-id="7fe77-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7fe77-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fe77-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fe77-125">Authorization</span></span>|<span data-ttu-id="7fe77-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fe77-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fe77-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7fe77-127">Accept</span></span>|<span data-ttu-id="7fe77-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7fe77-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe77-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe77-129">Request body</span></span>
<span data-ttu-id="7fe77-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fe77-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fe77-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe77-131">Response</span></span>
<span data-ttu-id="7fe77-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe77-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe77-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fe77-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fe77-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe77-134">Request</span></span>
<span data-ttu-id="7fe77-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe77-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="7fe77-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe77-136">Response</span></span>
<span data-ttu-id="7fe77-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





