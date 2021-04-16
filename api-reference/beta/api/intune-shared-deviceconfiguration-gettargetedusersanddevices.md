---
title: ação getTargetedUsersAndDevices
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b10470cc49152dcd683f6ea6024946e5ab52566
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863314"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="d49a2-103">ação getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="d49a2-103">getTargetedUsersAndDevices action</span></span>

<span data-ttu-id="d49a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d49a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d49a2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d49a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d49a2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d49a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d49a2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d49a2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d49a2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d49a2-108">Prerequisites</span></span>
<span data-ttu-id="d49a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d49a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d49a2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d49a2-111">Permission type</span></span>|<span data-ttu-id="d49a2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d49a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d49a2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d49a2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d49a2-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d49a2-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d49a2-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d49a2-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d49a2-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d49a2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d49a2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d49a2-117">Not supported.</span></span>|
|<span data-ttu-id="d49a2-118">Application</span><span class="sxs-lookup"><span data-stu-id="d49a2-118">Application</span></span>||
| <span data-ttu-id="d49a2-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d49a2-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d49a2-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d49a2-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d49a2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d49a2-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="d49a2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d49a2-122">Request headers</span></span>
|<span data-ttu-id="d49a2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d49a2-123">Header</span></span>|<span data-ttu-id="d49a2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d49a2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d49a2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d49a2-125">Authorization</span></span>|<span data-ttu-id="d49a2-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d49a2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d49a2-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d49a2-127">Accept</span></span>|<span data-ttu-id="d49a2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d49a2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d49a2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d49a2-129">Request body</span></span>
<span data-ttu-id="d49a2-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d49a2-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d49a2-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d49a2-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d49a2-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d49a2-132">Property</span></span>|<span data-ttu-id="d49a2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d49a2-133">Type</span></span>|<span data-ttu-id="d49a2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d49a2-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d49a2-135">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="d49a2-135">deviceConfigurationIds</span></span>|<span data-ttu-id="d49a2-136">String collection</span><span class="sxs-lookup"><span data-stu-id="d49a2-136">String collection</span></span>|<span data-ttu-id="d49a2-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d49a2-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d49a2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d49a2-138">Response</span></span>
<span data-ttu-id="d49a2-139">Se tiver êxito, essa ação retornará um código de resposta e uma coleção `200 OK` [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d49a2-139">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d49a2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d49a2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d49a2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d49a2-141">Request</span></span>
<span data-ttu-id="d49a2-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d49a2-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d49a2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d49a2-143">Response</span></span>
<span data-ttu-id="d49a2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d49a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







