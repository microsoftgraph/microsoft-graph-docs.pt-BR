---
title: Listar windowsUpdateStates
description: Listar Propriedades e relações dos objetos windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 46f6390efe60be5b3ea17092228142ccfd70f5a9
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085413"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="3c7b6-103">Listar windowsUpdateStates</span><span class="sxs-lookup"><span data-stu-id="3c7b6-103">List windowsUpdateStates</span></span>

> <span data-ttu-id="3c7b6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c7b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c7b6-106">Listar Propriedades e relações dos objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="3c7b6-106">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c7b6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c7b6-107">Prerequisites</span></span>
<span data-ttu-id="3c7b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c7b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c7b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c7b6-110">Permission type</span></span>|<span data-ttu-id="3c7b6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c7b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c7b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c7b6-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3c7b6-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3c7b6-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3c7b6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c7b6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="3c7b6-115">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="3c7b6-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="3c7b6-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c7b6-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3c7b6-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c7b6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c7b6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-118">Not supported.</span></span>|
|<span data-ttu-id="3c7b6-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c7b6-119">Application</span></span>||
| <span data-ttu-id="3c7b6-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3c7b6-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3c7b6-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c7b6-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="3c7b6-122">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="3c7b6-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="3c7b6-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c7b6-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c7b6-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c7b6-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="3c7b6-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c7b6-125">Request headers</span></span>
|<span data-ttu-id="3c7b6-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c7b6-126">Header</span></span>|<span data-ttu-id="3c7b6-127">Valor</span><span class="sxs-lookup"><span data-stu-id="3c7b6-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c7b6-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c7b6-128">Authorization</span></span>|<span data-ttu-id="3c7b6-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c7b6-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c7b6-130">Accept</span></span>|<span data-ttu-id="3c7b6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="3c7b6-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c7b6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c7b6-132">Request body</span></span>
<span data-ttu-id="3c7b6-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c7b6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c7b6-134">Response</span></span>
<span data-ttu-id="3c7b6-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-135">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c7b6-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c7b6-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c7b6-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c7b6-137">Request</span></span>
<span data-ttu-id="3c7b6-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="3c7b6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c7b6-139">Response</span></span>
<span data-ttu-id="3c7b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c7b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









