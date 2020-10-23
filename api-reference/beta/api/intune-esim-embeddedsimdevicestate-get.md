---
title: Obter embeddedSIMDeviceState
description: Leia as propriedades e as relações do objeto embeddedSIMDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: caef92326fb76144a46e2cdc051a3aef4ae82342
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693063"
---
# <a name="get-embeddedsimdevicestate"></a><span data-ttu-id="a8e45-103">Obter embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="a8e45-103">Get embeddedSIMDeviceState</span></span>

<span data-ttu-id="a8e45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8e45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8e45-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8e45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8e45-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8e45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8e45-107">Leia as propriedades e as relações do objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a8e45-107">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8e45-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8e45-108">Prerequisites</span></span>
<span data-ttu-id="a8e45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8e45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8e45-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8e45-111">Permission type</span></span>|<span data-ttu-id="a8e45-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8e45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8e45-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8e45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8e45-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8e45-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a8e45-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8e45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8e45-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8e45-116">Not supported.</span></span>|
|<span data-ttu-id="a8e45-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8e45-117">Application</span></span>|<span data-ttu-id="a8e45-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8e45-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8e45-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8e45-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8e45-120">Optional query parameters</span></span>
<span data-ttu-id="a8e45-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e45-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8e45-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e45-122">Request headers</span></span>
|<span data-ttu-id="a8e45-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8e45-123">Header</span></span>|<span data-ttu-id="a8e45-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a8e45-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8e45-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8e45-125">Authorization</span></span>|<span data-ttu-id="a8e45-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8e45-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8e45-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8e45-127">Accept</span></span>|<span data-ttu-id="a8e45-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a8e45-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8e45-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e45-129">Request body</span></span>
<span data-ttu-id="a8e45-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8e45-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8e45-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e45-131">Response</span></span>
<span data-ttu-id="a8e45-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e45-132">If successful, this method returns a `200 OK` response code and [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e45-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8e45-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8e45-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e45-134">Request</span></span>
<span data-ttu-id="a8e45-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8e45-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="a8e45-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e45-136">Response</span></span>
<span data-ttu-id="a8e45-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8e45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
    "id": "908884a3-84a3-9088-a384-8890a3848890",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
    "deviceName": "Device Name value",
    "userName": "User Name value",
    "state": "failed",
    "stateDetails": "State Details value"
  }
}
```





