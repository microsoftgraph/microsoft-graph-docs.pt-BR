---
title: Listar windowsUpdateStates
description: Listar Propriedades e relações dos objetos windowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d7839ca7c75cf2c401bfc881c7504651d33f961e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735327"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="4e407-103">Listar windowsUpdateStates</span><span class="sxs-lookup"><span data-stu-id="4e407-103">List windowsUpdateStates</span></span>

<span data-ttu-id="4e407-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e407-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e407-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e407-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e407-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e407-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e407-107">Listar Propriedades e relações dos objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="4e407-107">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e407-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e407-108">Prerequisites</span></span>
<span data-ttu-id="4e407-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e407-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e407-111">Permission type</span></span>|<span data-ttu-id="4e407-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e407-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e407-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e407-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4e407-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4e407-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4e407-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e407-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4e407-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="4e407-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4e407-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e407-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e407-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e407-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e407-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e407-119">Not supported.</span></span>|
|<span data-ttu-id="4e407-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e407-120">Application</span></span>||
| <span data-ttu-id="4e407-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4e407-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4e407-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e407-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4e407-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="4e407-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4e407-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e407-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e407-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e407-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="4e407-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e407-126">Request headers</span></span>
|<span data-ttu-id="4e407-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e407-127">Header</span></span>|<span data-ttu-id="4e407-128">Valor</span><span class="sxs-lookup"><span data-stu-id="4e407-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e407-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e407-129">Authorization</span></span>|<span data-ttu-id="4e407-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e407-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e407-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e407-131">Accept</span></span>|<span data-ttu-id="4e407-132">application/json</span><span class="sxs-lookup"><span data-stu-id="4e407-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e407-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e407-133">Request body</span></span>
<span data-ttu-id="4e407-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e407-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e407-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e407-135">Response</span></span>
<span data-ttu-id="4e407-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e407-136">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e407-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e407-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e407-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e407-138">Request</span></span>
<span data-ttu-id="4e407-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e407-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="4e407-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e407-140">Response</span></span>
<span data-ttu-id="4e407-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e407-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








