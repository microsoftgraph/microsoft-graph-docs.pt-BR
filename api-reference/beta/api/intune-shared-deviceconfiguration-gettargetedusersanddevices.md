---
title: ação getTargetedUsersAndDevices
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3f12db1dc4d7023846c26e7824041470371dc26
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537047"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="0ae41-103">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="0ae41-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="0ae41-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ae41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ae41-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ae41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ae41-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0ae41-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ae41-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ae41-107">Prerequisites</span></span>
<span data-ttu-id="0ae41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ae41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ae41-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ae41-110">Permission type</span></span>|<span data-ttu-id="0ae41-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ae41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ae41-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ae41-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0ae41-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0ae41-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0ae41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ae41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0ae41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ae41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ae41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ae41-116">Not supported.</span></span>|
|<span data-ttu-id="0ae41-117">Application</span><span class="sxs-lookup"><span data-stu-id="0ae41-117">Application</span></span>||
| <span data-ttu-id="0ae41-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0ae41-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0ae41-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ae41-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ae41-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ae41-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="0ae41-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae41-121">Request headers</span></span>
|<span data-ttu-id="0ae41-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ae41-122">Header</span></span>|<span data-ttu-id="0ae41-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0ae41-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ae41-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ae41-124">Authorization</span></span>|<span data-ttu-id="0ae41-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ae41-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ae41-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ae41-126">Accept</span></span>|<span data-ttu-id="0ae41-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0ae41-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ae41-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae41-128">Request body</span></span>
<span data-ttu-id="0ae41-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0ae41-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0ae41-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0ae41-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0ae41-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ae41-131">Property</span></span>|<span data-ttu-id="0ae41-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ae41-132">Type</span></span>|<span data-ttu-id="0ae41-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ae41-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ae41-134">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="0ae41-134">deviceConfigurationIds</span></span>|<span data-ttu-id="0ae41-135">String collection</span><span class="sxs-lookup"><span data-stu-id="0ae41-135">String collection</span></span>|<span data-ttu-id="0ae41-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0ae41-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0ae41-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ae41-137">Response</span></span>
<span data-ttu-id="0ae41-138">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ae41-138">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ae41-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ae41-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ae41-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae41-140">Request</span></span>
<span data-ttu-id="0ae41-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ae41-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ae41-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ae41-142">Response</span></span>
<span data-ttu-id="0ae41-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ae41-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






