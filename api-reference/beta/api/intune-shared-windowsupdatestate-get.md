---
title: Obter windowsUpdateState
description: Leia as propriedades e as relações do objeto windowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11eed22457710383a16bf43f4be697db1bd31286
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966986"
---
# <a name="get-windowsupdatestate"></a><span data-ttu-id="b9319-103">Obter windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="b9319-103">Get windowsUpdateState</span></span>

<span data-ttu-id="b9319-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9319-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9319-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9319-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9319-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9319-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9319-107">Leia as propriedades e as relações do objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="b9319-107">Read properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9319-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9319-108">Prerequisites</span></span>
<span data-ttu-id="b9319-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9319-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9319-111">Permission type</span></span>|<span data-ttu-id="b9319-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9319-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9319-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9319-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b9319-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b9319-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b9319-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9319-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b9319-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="b9319-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="b9319-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9319-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9319-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9319-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9319-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9319-119">Not supported.</span></span>|
|<span data-ttu-id="b9319-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9319-120">Application</span></span>||
| <span data-ttu-id="b9319-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b9319-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b9319-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9319-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b9319-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="b9319-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="b9319-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9319-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9319-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9319-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9319-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9319-126">Optional query parameters</span></span>
<span data-ttu-id="b9319-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9319-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9319-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9319-128">Request headers</span></span>
|<span data-ttu-id="b9319-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9319-129">Header</span></span>|<span data-ttu-id="b9319-130">Valor</span><span class="sxs-lookup"><span data-stu-id="b9319-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9319-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9319-131">Authorization</span></span>|<span data-ttu-id="b9319-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9319-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9319-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9319-133">Accept</span></span>|<span data-ttu-id="b9319-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b9319-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9319-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9319-135">Request body</span></span>
<span data-ttu-id="b9319-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9319-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9319-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9319-137">Response</span></span>
<span data-ttu-id="b9319-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9319-138">If successful, this method returns a `200 OK` response code and [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9319-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9319-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9319-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9319-140">Request</span></span>
<span data-ttu-id="b9319-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9319-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="b9319-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9319-142">Response</span></span>
<span data-ttu-id="b9319-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9319-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









