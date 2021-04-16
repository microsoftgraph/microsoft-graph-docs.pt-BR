---
title: Obter windowsUpdateState
description: Ler propriedades e relações do objeto windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2cee690d2bb85161ca9b645bf91280df81db2de
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864750"
---
# <a name="get-windowsupdatestate"></a><span data-ttu-id="25b4a-103">Obter windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="25b4a-103">Get windowsUpdateState</span></span>

<span data-ttu-id="25b4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25b4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25b4a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25b4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25b4a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25b4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b4a-107">Ler propriedades e relações do [objeto windowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="25b4a-107">Read properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25b4a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25b4a-108">Prerequisites</span></span>
<span data-ttu-id="25b4a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25b4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25b4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25b4a-111">Permission type</span></span>|<span data-ttu-id="25b4a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25b4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25b4a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25b4a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="25b4a-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="25b4a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="25b4a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25b4a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="25b4a-116">&nbsp;&nbsp; **Atualização de Software**</span><span class="sxs-lookup"><span data-stu-id="25b4a-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="25b4a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25b4a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="25b4a-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25b4a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25b4a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25b4a-119">Not supported.</span></span>|
|<span data-ttu-id="25b4a-120">Application</span><span class="sxs-lookup"><span data-stu-id="25b4a-120">Application</span></span>||
| <span data-ttu-id="25b4a-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="25b4a-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="25b4a-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25b4a-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="25b4a-123">&nbsp;&nbsp; **Atualização de Software**</span><span class="sxs-lookup"><span data-stu-id="25b4a-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="25b4a-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25b4a-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25b4a-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25b4a-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25b4a-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25b4a-126">Optional query parameters</span></span>
<span data-ttu-id="25b4a-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25b4a-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25b4a-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25b4a-128">Request headers</span></span>
|<span data-ttu-id="25b4a-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25b4a-129">Header</span></span>|<span data-ttu-id="25b4a-130">Valor</span><span class="sxs-lookup"><span data-stu-id="25b4a-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25b4a-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="25b4a-131">Authorization</span></span>|<span data-ttu-id="25b4a-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25b4a-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25b4a-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25b4a-133">Accept</span></span>|<span data-ttu-id="25b4a-134">application/json</span><span class="sxs-lookup"><span data-stu-id="25b4a-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25b4a-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25b4a-135">Request body</span></span>
<span data-ttu-id="25b4a-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25b4a-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25b4a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="25b4a-137">Response</span></span>
<span data-ttu-id="25b4a-138">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25b4a-138">If successful, this method returns a `200 OK` response code and [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25b4a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25b4a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="25b4a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25b4a-140">Request</span></span>
<span data-ttu-id="25b4a-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25b4a-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="25b4a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="25b4a-142">Response</span></span>
<span data-ttu-id="25b4a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25b4a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







