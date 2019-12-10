---
title: Listar windowsUpdateStates
description: Listar Propriedades e relações dos objetos windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d242af4a368aafb414b3224e93a8340ff1370a67
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939315"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="b2b18-103">Listar windowsUpdateStates</span><span class="sxs-lookup"><span data-stu-id="b2b18-103">List windowsUpdateStates</span></span>

> <span data-ttu-id="b2b18-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2b18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2b18-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2b18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2b18-106">Listar Propriedades e relações dos objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="b2b18-106">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2b18-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2b18-107">Prerequisites</span></span>
<span data-ttu-id="b2b18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2b18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2b18-110">Permission type</span></span>|<span data-ttu-id="b2b18-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2b18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2b18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2b18-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b2b18-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b2b18-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b2b18-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2b18-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b2b18-115">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="b2b18-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="b2b18-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2b18-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b2b18-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2b18-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2b18-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2b18-118">Not supported.</span></span>|
|<span data-ttu-id="b2b18-119">Application</span><span class="sxs-lookup"><span data-stu-id="b2b18-119">Application</span></span>||
| <span data-ttu-id="b2b18-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b2b18-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b2b18-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2b18-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b2b18-122">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="b2b18-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="b2b18-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2b18-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2b18-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2b18-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="b2b18-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2b18-125">Request headers</span></span>
|<span data-ttu-id="b2b18-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2b18-126">Header</span></span>|<span data-ttu-id="b2b18-127">Valor</span><span class="sxs-lookup"><span data-stu-id="b2b18-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2b18-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2b18-128">Authorization</span></span>|<span data-ttu-id="b2b18-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2b18-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2b18-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2b18-130">Accept</span></span>|<span data-ttu-id="b2b18-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b2b18-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2b18-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2b18-132">Request body</span></span>
<span data-ttu-id="b2b18-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2b18-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2b18-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2b18-134">Response</span></span>
<span data-ttu-id="b2b18-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2b18-135">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b18-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2b18-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2b18-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2b18-137">Request</span></span>
<span data-ttu-id="b2b18-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2b18-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="b2b18-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2b18-139">Response</span></span>
<span data-ttu-id="b2b18-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2b18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 630

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateState",
      "id": "3d92af00-af00-3d92-00af-923d00af923d",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "status": "pendingInstallation",
      "qualityUpdateVersion": "Quality Update Version value",
      "featureUpdateVersion": "Feature Update Version value",
      "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
    }
  ]
}
```








