---
title: Obter windowsUpdateState
description: Leia as propriedades e as relações do objeto windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 65239dadba20d14c8a4508e38215cc147ca46ad5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199517"
---
# <a name="get-windowsupdatestate"></a><span data-ttu-id="7a5ad-103">Obter windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="7a5ad-103">Get windowsUpdateState</span></span>

> <span data-ttu-id="7a5ad-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a5ad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a5ad-106">Leia as propriedades e as relações do objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="7a5ad-106">Read properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a5ad-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a5ad-107">Prerequisites</span></span>
<span data-ttu-id="7a5ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a5ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a5ad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a5ad-110">Permission type</span></span>|<span data-ttu-id="7a5ad-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a5ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a5ad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a5ad-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7a5ad-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7a5ad-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7a5ad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a5ad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="7a5ad-115">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="7a5ad-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="7a5ad-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a5ad-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a5ad-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a5ad-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a5ad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-118">Not supported.</span></span>|
|<span data-ttu-id="7a5ad-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a5ad-119">Application</span></span>||
| <span data-ttu-id="7a5ad-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="7a5ad-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7a5ad-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a5ad-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="7a5ad-122">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="7a5ad-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="7a5ad-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a5ad-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a5ad-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a5ad-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a5ad-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a5ad-125">Optional query parameters</span></span>
<span data-ttu-id="7a5ad-126">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a5ad-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a5ad-127">Request headers</span></span>
|<span data-ttu-id="7a5ad-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a5ad-128">Header</span></span>|<span data-ttu-id="7a5ad-129">Valor</span><span class="sxs-lookup"><span data-stu-id="7a5ad-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a5ad-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a5ad-130">Authorization</span></span>|<span data-ttu-id="7a5ad-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a5ad-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a5ad-132">Accept</span></span>|<span data-ttu-id="7a5ad-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7a5ad-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a5ad-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a5ad-134">Request body</span></span>
<span data-ttu-id="7a5ad-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a5ad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a5ad-136">Response</span></span>
<span data-ttu-id="7a5ad-137">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-137">If successful, this method returns a `200 OK` response code and [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a5ad-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a5ad-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a5ad-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a5ad-139">Request</span></span>
<span data-ttu-id="7a5ad-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="7a5ad-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a5ad-141">Response</span></span>
<span data-ttu-id="7a5ad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a5ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "value": {
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
}
```




