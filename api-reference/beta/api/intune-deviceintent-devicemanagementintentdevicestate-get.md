---
title: Obter deviceManagementIntentDeviceState
description: Leia as propriedades e as relações do objeto deviceManagementIntentDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11609a810ab5ed10db9bb18569ceb7f0d2a497fd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915694"
---
# <a name="get-devicemanagementintentdevicestate"></a><span data-ttu-id="f06e6-103">Obter deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="f06e6-103">Get deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="f06e6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f06e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f06e6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f06e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f06e6-106">Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="f06e6-106">Read properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f06e6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f06e6-107">Prerequisites</span></span>
<span data-ttu-id="f06e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f06e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f06e6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f06e6-110">Permission type</span></span>|<span data-ttu-id="f06e6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f06e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f06e6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f06e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f06e6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f06e6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f06e6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f06e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f06e6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f06e6-115">Not supported.</span></span>|
|<span data-ttu-id="f06e6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f06e6-116">Application</span></span>|<span data-ttu-id="f06e6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f06e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f06e6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f06e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f06e6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f06e6-119">Optional query parameters</span></span>
<span data-ttu-id="f06e6-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f06e6-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f06e6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f06e6-121">Request headers</span></span>
|<span data-ttu-id="f06e6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f06e6-122">Header</span></span>|<span data-ttu-id="f06e6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f06e6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f06e6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f06e6-124">Authorization</span></span>|<span data-ttu-id="f06e6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f06e6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f06e6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f06e6-126">Accept</span></span>|<span data-ttu-id="f06e6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f06e6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f06e6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f06e6-128">Request body</span></span>
<span data-ttu-id="f06e6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f06e6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f06e6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f06e6-130">Response</span></span>
<span data-ttu-id="f06e6-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f06e6-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f06e6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f06e6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f06e6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f06e6-133">Request</span></span>
<span data-ttu-id="f06e6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f06e6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="f06e6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f06e6-135">Response</span></span>
<span data-ttu-id="f06e6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f06e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 426

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
    "id": "8db75881-5881-8db7-8158-b78d8158b78d",
    "userPrincipalName": "User Principal Name value",
    "userName": "User Name value",
    "deviceDisplayName": "Device Display Name value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "state": "notApplicable",
    "deviceId": "Device Id value"
  }
}
```




