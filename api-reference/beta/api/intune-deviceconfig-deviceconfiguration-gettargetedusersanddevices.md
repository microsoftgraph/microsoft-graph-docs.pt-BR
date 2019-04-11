---
title: ação getTargetedUsersAndDevices
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 128e0d63cfc2c613eb0ee16e4cf0a82d0e0c32e8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793123"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="af33a-103">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="af33a-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="af33a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="af33a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af33a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af33a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af33a-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="af33a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af33a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af33a-107">Prerequisites</span></span>
<span data-ttu-id="af33a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af33a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af33a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af33a-110">Permission type</span></span>|<span data-ttu-id="af33a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af33a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af33a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af33a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af33a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af33a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="af33a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af33a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af33a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af33a-115">Not supported.</span></span>|
|<span data-ttu-id="af33a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af33a-116">Application</span></span>|<span data-ttu-id="af33a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af33a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af33a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af33a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="af33a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af33a-119">Request headers</span></span>
|<span data-ttu-id="af33a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af33a-120">Header</span></span>|<span data-ttu-id="af33a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="af33a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af33a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="af33a-122">Authorization</span></span>|<span data-ttu-id="af33a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af33a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af33a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af33a-124">Accept</span></span>|<span data-ttu-id="af33a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af33a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af33a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af33a-126">Request body</span></span>
<span data-ttu-id="af33a-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="af33a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="af33a-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="af33a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="af33a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af33a-129">Property</span></span>|<span data-ttu-id="af33a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="af33a-130">Type</span></span>|<span data-ttu-id="af33a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="af33a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af33a-132">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="af33a-132">deviceConfigurationIds</span></span>|<span data-ttu-id="af33a-133">String collection</span><span class="sxs-lookup"><span data-stu-id="af33a-133">String collection</span></span>|<span data-ttu-id="af33a-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="af33a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="af33a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="af33a-135">Response</span></span>
<span data-ttu-id="af33a-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af33a-136">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af33a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af33a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="af33a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af33a-138">Request</span></span>
<span data-ttu-id="af33a-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af33a-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af33a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="af33a-140">Response</span></span>
<span data-ttu-id="af33a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af33a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





