---
title: Listar embeddedSIMDeviceStates
description: Listar Propriedades e relações dos objetos embeddedSIMDeviceState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06a7a51cadf2094f8182cb4bae4dfdbc7e291c95
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465965"
---
# <a name="list-embeddedsimdevicestates"></a><span data-ttu-id="74a07-103">Listar embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="74a07-103">List embeddedSIMDeviceStates</span></span>

<span data-ttu-id="74a07-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="74a07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74a07-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74a07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74a07-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74a07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74a07-107">Listar Propriedades e relações dos objetos [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="74a07-107">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74a07-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74a07-108">Prerequisites</span></span>
<span data-ttu-id="74a07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74a07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74a07-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74a07-111">Permission type</span></span>|<span data-ttu-id="74a07-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74a07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74a07-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74a07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74a07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="74a07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="74a07-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74a07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74a07-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74a07-116">Not supported.</span></span>|
|<span data-ttu-id="74a07-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74a07-117">Application</span></span>|<span data-ttu-id="74a07-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="74a07-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74a07-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74a07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="74a07-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74a07-120">Request headers</span></span>
|<span data-ttu-id="74a07-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74a07-121">Header</span></span>|<span data-ttu-id="74a07-122">Valor</span><span class="sxs-lookup"><span data-stu-id="74a07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74a07-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="74a07-123">Authorization</span></span>|<span data-ttu-id="74a07-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74a07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74a07-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74a07-125">Accept</span></span>|<span data-ttu-id="74a07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74a07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74a07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74a07-127">Request body</span></span>
<span data-ttu-id="74a07-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74a07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74a07-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="74a07-129">Response</span></span>
<span data-ttu-id="74a07-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74a07-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74a07-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74a07-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="74a07-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74a07-132">Request</span></span>
<span data-ttu-id="74a07-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74a07-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="74a07-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="74a07-134">Response</span></span>
<span data-ttu-id="74a07-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74a07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "value": [
    {
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
  ]
}
```





