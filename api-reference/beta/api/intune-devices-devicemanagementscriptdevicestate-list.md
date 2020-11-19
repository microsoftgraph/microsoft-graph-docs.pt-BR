---
title: Listar deviceManagementScriptDeviceStates
description: Listar Propriedades e relações dos objetos deviceManagementScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f93ede247823ccefb4fc5e331835307efe6c948
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212885"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="4b112-103">Listar deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="4b112-103">List deviceManagementScriptDeviceStates</span></span>

<span data-ttu-id="4b112-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b112-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b112-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b112-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b112-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b112-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b112-107">Listar Propriedades e relações dos objetos [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="4b112-107">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b112-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b112-108">Prerequisites</span></span>
<span data-ttu-id="4b112-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b112-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b112-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b112-111">Permission type</span></span>|<span data-ttu-id="4b112-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b112-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b112-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b112-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b112-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b112-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4b112-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b112-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b112-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b112-116">Not supported.</span></span>|
|<span data-ttu-id="4b112-117">Application</span><span class="sxs-lookup"><span data-stu-id="4b112-117">Application</span></span>|<span data-ttu-id="4b112-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b112-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b112-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b112-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="4b112-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b112-120">Request headers</span></span>
|<span data-ttu-id="4b112-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b112-121">Header</span></span>|<span data-ttu-id="4b112-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b112-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b112-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b112-123">Authorization</span></span>|<span data-ttu-id="4b112-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b112-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b112-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b112-125">Accept</span></span>|<span data-ttu-id="4b112-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b112-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b112-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b112-127">Request body</span></span>
<span data-ttu-id="4b112-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b112-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b112-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b112-129">Response</span></span>
<span data-ttu-id="4b112-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b112-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b112-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b112-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b112-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b112-132">Request</span></span>
<span data-ttu-id="4b112-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b112-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="4b112-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b112-134">Response</span></span>
<span data-ttu-id="4b112-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b112-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
      "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
      "runState": "success",
      "resultMessage": "Result Message value",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "errorCode": 9,
      "errorDescription": "Error Description value"
    }
  ]
}
```




