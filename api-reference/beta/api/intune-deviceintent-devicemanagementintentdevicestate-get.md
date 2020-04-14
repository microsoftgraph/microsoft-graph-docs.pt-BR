---
title: Obter deviceManagementIntentDeviceState
description: Leia as propriedades e as relações do objeto deviceManagementIntentDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3691efda09e6aed92111bc1a57d0bed96df611ae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43326328"
---
# <a name="get-devicemanagementintentdevicestate"></a><span data-ttu-id="2add4-103">Obter deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="2add4-103">Get deviceManagementIntentDeviceState</span></span>

<span data-ttu-id="2add4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2add4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2add4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2add4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2add4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2add4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2add4-107">Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="2add4-107">Read properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2add4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2add4-108">Prerequisites</span></span>
<span data-ttu-id="2add4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2add4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2add4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2add4-111">Permission type</span></span>|<span data-ttu-id="2add4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2add4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2add4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2add4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2add4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2add4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2add4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2add4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2add4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2add4-116">Not supported.</span></span>|
|<span data-ttu-id="2add4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2add4-117">Application</span></span>|<span data-ttu-id="2add4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2add4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2add4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2add4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2add4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2add4-120">Optional query parameters</span></span>
<span data-ttu-id="2add4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2add4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2add4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2add4-122">Request headers</span></span>
|<span data-ttu-id="2add4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2add4-123">Header</span></span>|<span data-ttu-id="2add4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2add4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2add4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2add4-125">Authorization</span></span>|<span data-ttu-id="2add4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2add4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2add4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2add4-127">Accept</span></span>|<span data-ttu-id="2add4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2add4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2add4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2add4-129">Request body</span></span>
<span data-ttu-id="2add4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2add4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2add4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2add4-131">Response</span></span>
<span data-ttu-id="2add4-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2add4-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2add4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2add4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2add4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2add4-134">Request</span></span>
<span data-ttu-id="2add4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2add4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="2add4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2add4-136">Response</span></span>
<span data-ttu-id="2add4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2add4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



