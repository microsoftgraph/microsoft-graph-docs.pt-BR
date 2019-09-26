---
title: ação getTargetedUsersAndDevices
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bee4879dba43f3d21a16e25ee316eb991d0f1ba8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199451"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="92b79-103">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="92b79-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="92b79-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92b79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92b79-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92b79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92b79-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92b79-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92b79-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92b79-107">Prerequisites</span></span>
<span data-ttu-id="92b79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b79-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92b79-110">Permission type</span></span>|<span data-ttu-id="92b79-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92b79-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92b79-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92b79-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="92b79-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="92b79-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="92b79-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b79-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92b79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92b79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92b79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92b79-116">Not supported.</span></span>|
|<span data-ttu-id="92b79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92b79-117">Application</span></span>||
| <span data-ttu-id="92b79-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="92b79-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="92b79-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b79-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92b79-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92b79-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="92b79-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92b79-121">Request headers</span></span>
|<span data-ttu-id="92b79-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92b79-122">Header</span></span>|<span data-ttu-id="92b79-123">Valor</span><span class="sxs-lookup"><span data-stu-id="92b79-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92b79-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="92b79-124">Authorization</span></span>|<span data-ttu-id="92b79-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92b79-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92b79-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92b79-126">Accept</span></span>|<span data-ttu-id="92b79-127">application/json</span><span class="sxs-lookup"><span data-stu-id="92b79-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b79-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92b79-128">Request body</span></span>
<span data-ttu-id="92b79-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="92b79-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="92b79-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="92b79-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="92b79-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92b79-131">Property</span></span>|<span data-ttu-id="92b79-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="92b79-132">Type</span></span>|<span data-ttu-id="92b79-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="92b79-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92b79-134">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="92b79-134">deviceConfigurationIds</span></span>|<span data-ttu-id="92b79-135">String collection</span><span class="sxs-lookup"><span data-stu-id="92b79-135">String collection</span></span>|<span data-ttu-id="92b79-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92b79-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="92b79-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="92b79-137">Response</span></span>
<span data-ttu-id="92b79-138">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92b79-138">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92b79-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92b79-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="92b79-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92b79-140">Request</span></span>
<span data-ttu-id="92b79-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92b79-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/getTargetedUsersAndDevices

Content-type: application/json
Content-length: 78

{
  "deviceConfigurationIds": [
    "Device Configuration Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="92b79-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="92b79-142">Response</span></span>
<span data-ttu-id="92b79-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92b79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
    }
  ]
}
```




