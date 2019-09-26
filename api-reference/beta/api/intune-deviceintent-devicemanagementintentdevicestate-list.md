---
title: Listar deviceManagementIntentDeviceStates
description: Listar Propriedades e relações dos objetos deviceManagementIntentDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ea0051e2b0fea2a442bd8e9392571af875783af
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180878"
---
# <a name="list-devicemanagementintentdevicestates"></a><span data-ttu-id="dae51-103">Listar deviceManagementIntentDeviceStates</span><span class="sxs-lookup"><span data-stu-id="dae51-103">List deviceManagementIntentDeviceStates</span></span>

> <span data-ttu-id="dae51-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dae51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dae51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dae51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dae51-106">Listar Propriedades e relações dos objetos [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="dae51-106">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dae51-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dae51-107">Prerequisites</span></span>
<span data-ttu-id="dae51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dae51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dae51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dae51-110">Permission type</span></span>|<span data-ttu-id="dae51-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dae51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dae51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dae51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dae51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dae51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dae51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dae51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dae51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dae51-115">Not supported.</span></span>|
|<span data-ttu-id="dae51-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dae51-116">Application</span></span>|<span data-ttu-id="dae51-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dae51-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dae51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dae51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="dae51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dae51-119">Request headers</span></span>
|<span data-ttu-id="dae51-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dae51-120">Header</span></span>|<span data-ttu-id="dae51-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dae51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dae51-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dae51-122">Authorization</span></span>|<span data-ttu-id="dae51-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dae51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dae51-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dae51-124">Accept</span></span>|<span data-ttu-id="dae51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dae51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dae51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dae51-126">Request body</span></span>
<span data-ttu-id="dae51-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dae51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dae51-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae51-128">Response</span></span>
<span data-ttu-id="dae51-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dae51-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dae51-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dae51-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dae51-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dae51-131">Request</span></span>
<span data-ttu-id="dae51-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dae51-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="dae51-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae51-133">Response</span></span>
<span data-ttu-id="dae51-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dae51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 456

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
      "id": "8db75881-5881-8db7-8158-b78d8158b78d",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceDisplayName": "Device Display Name value",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "state": "notApplicable",
      "deviceId": "Device Id value"
    }
  ]
}
```




