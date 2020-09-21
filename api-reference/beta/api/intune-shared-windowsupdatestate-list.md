---
title: Listar windowsUpdateStates
description: Listar Propriedades e relações dos objetos windowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7a45cb9a7c38b9be5095d083f7af9910cff923a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966951"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="3f97f-103">Listar windowsUpdateStates</span><span class="sxs-lookup"><span data-stu-id="3f97f-103">List windowsUpdateStates</span></span>

<span data-ttu-id="3f97f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f97f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f97f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f97f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f97f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f97f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f97f-107">Listar Propriedades e relações dos objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="3f97f-107">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f97f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3f97f-108">Prerequisites</span></span>
<span data-ttu-id="3f97f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f97f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f97f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f97f-111">Permission type</span></span>|<span data-ttu-id="3f97f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3f97f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f97f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f97f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3f97f-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3f97f-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3f97f-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f97f-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="3f97f-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="3f97f-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="3f97f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f97f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3f97f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f97f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f97f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f97f-119">Not supported.</span></span>|
|<span data-ttu-id="3f97f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f97f-120">Application</span></span>||
| <span data-ttu-id="3f97f-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3f97f-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3f97f-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f97f-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="3f97f-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="3f97f-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="3f97f-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f97f-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f97f-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f97f-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="3f97f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f97f-126">Request headers</span></span>
|<span data-ttu-id="3f97f-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f97f-127">Header</span></span>|<span data-ttu-id="3f97f-128">Valor</span><span class="sxs-lookup"><span data-stu-id="3f97f-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f97f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f97f-129">Authorization</span></span>|<span data-ttu-id="3f97f-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f97f-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f97f-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3f97f-131">Accept</span></span>|<span data-ttu-id="3f97f-132">application/json</span><span class="sxs-lookup"><span data-stu-id="3f97f-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f97f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f97f-133">Request body</span></span>
<span data-ttu-id="3f97f-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f97f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f97f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f97f-135">Response</span></span>
<span data-ttu-id="3f97f-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f97f-136">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f97f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f97f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f97f-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f97f-138">Request</span></span>
<span data-ttu-id="3f97f-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f97f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="3f97f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f97f-140">Response</span></span>
<span data-ttu-id="3f97f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f97f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









