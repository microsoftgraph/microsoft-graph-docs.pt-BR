---
title: Obter windowsUpdateState
description: Leia as propriedades e as relações do objeto windowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f2902dd26b3be6c241fd6646b9a56364645bef6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735334"
---
# <a name="get-windowsupdatestate"></a><span data-ttu-id="21a10-103">Obter windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="21a10-103">Get windowsUpdateState</span></span>

<span data-ttu-id="21a10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21a10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21a10-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21a10-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21a10-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21a10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21a10-107">Leia as propriedades e as relações do objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="21a10-107">Read properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21a10-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21a10-108">Prerequisites</span></span>
<span data-ttu-id="21a10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21a10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21a10-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21a10-111">Permission type</span></span>|<span data-ttu-id="21a10-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21a10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21a10-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21a10-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="21a10-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="21a10-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="21a10-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21a10-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="21a10-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="21a10-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="21a10-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21a10-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="21a10-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21a10-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21a10-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21a10-119">Not supported.</span></span>|
|<span data-ttu-id="21a10-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21a10-120">Application</span></span>||
| <span data-ttu-id="21a10-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="21a10-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="21a10-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21a10-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="21a10-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="21a10-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="21a10-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21a10-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21a10-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21a10-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21a10-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21a10-126">Optional query parameters</span></span>
<span data-ttu-id="21a10-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="21a10-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21a10-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21a10-128">Request headers</span></span>
|<span data-ttu-id="21a10-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21a10-129">Header</span></span>|<span data-ttu-id="21a10-130">Valor</span><span class="sxs-lookup"><span data-stu-id="21a10-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21a10-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="21a10-131">Authorization</span></span>|<span data-ttu-id="21a10-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21a10-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21a10-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21a10-133">Accept</span></span>|<span data-ttu-id="21a10-134">application/json</span><span class="sxs-lookup"><span data-stu-id="21a10-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21a10-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21a10-135">Request body</span></span>
<span data-ttu-id="21a10-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21a10-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21a10-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="21a10-137">Response</span></span>
<span data-ttu-id="21a10-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21a10-138">If successful, this method returns a `200 OK` response code and [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21a10-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21a10-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="21a10-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21a10-140">Request</span></span>
<span data-ttu-id="21a10-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21a10-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="21a10-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="21a10-142">Response</span></span>
<span data-ttu-id="21a10-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21a10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








