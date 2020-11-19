---
title: Listar deviceManagementIntentDeviceStates
description: Listar Propriedades e relações dos objetos deviceManagementIntentDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e178f9b3a2d8c15ef20d728d1d6906d8d4e2763
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213081"
---
# <a name="list-devicemanagementintentdevicestates"></a><span data-ttu-id="f46df-103">Listar deviceManagementIntentDeviceStates</span><span class="sxs-lookup"><span data-stu-id="f46df-103">List deviceManagementIntentDeviceStates</span></span>

<span data-ttu-id="f46df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f46df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f46df-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f46df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f46df-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f46df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f46df-107">Listar Propriedades e relações dos objetos [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="f46df-107">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f46df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f46df-108">Prerequisites</span></span>
<span data-ttu-id="f46df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f46df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f46df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f46df-111">Permission type</span></span>|<span data-ttu-id="f46df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f46df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f46df-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f46df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f46df-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f46df-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f46df-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f46df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f46df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f46df-116">Not supported.</span></span>|
|<span data-ttu-id="f46df-117">Application</span><span class="sxs-lookup"><span data-stu-id="f46df-117">Application</span></span>|<span data-ttu-id="f46df-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f46df-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f46df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f46df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="f46df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f46df-120">Request headers</span></span>
|<span data-ttu-id="f46df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f46df-121">Header</span></span>|<span data-ttu-id="f46df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f46df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f46df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f46df-123">Authorization</span></span>|<span data-ttu-id="f46df-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f46df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f46df-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f46df-125">Accept</span></span>|<span data-ttu-id="f46df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f46df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f46df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f46df-127">Request body</span></span>
<span data-ttu-id="f46df-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f46df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f46df-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f46df-129">Response</span></span>
<span data-ttu-id="f46df-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f46df-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f46df-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f46df-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f46df-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f46df-132">Request</span></span>
<span data-ttu-id="f46df-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f46df-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="f46df-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f46df-134">Response</span></span>
<span data-ttu-id="f46df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f46df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




