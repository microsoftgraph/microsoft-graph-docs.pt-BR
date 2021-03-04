---
title: Listar userExperienceAnalyticsRemoteConnections
description: Listar propriedades e relações dos objetos userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7721ff94819c85e1fcb4fca4a86fc166e7e9a742
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445913"
---
# <a name="list-userexperienceanalyticsremoteconnections"></a><span data-ttu-id="c13f1-103">Listar userExperienceAnalyticsRemoteConnections</span><span class="sxs-lookup"><span data-stu-id="c13f1-103">List userExperienceAnalyticsRemoteConnections</span></span>

<span data-ttu-id="c13f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c13f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c13f1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c13f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c13f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c13f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c13f1-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="c13f1-107">List properties and relationships of the [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c13f1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c13f1-108">Prerequisites</span></span>
<span data-ttu-id="c13f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c13f1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c13f1-111">Permission type</span></span>|<span data-ttu-id="c13f1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c13f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c13f1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c13f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c13f1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c13f1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c13f1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c13f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c13f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c13f1-116">Not supported.</span></span>|
|<span data-ttu-id="c13f1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c13f1-117">Application</span></span>|<span data-ttu-id="c13f1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c13f1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c13f1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c13f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRemoteConnection
```

## <a name="request-headers"></a><span data-ttu-id="c13f1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f1-120">Request headers</span></span>
|<span data-ttu-id="c13f1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c13f1-121">Header</span></span>|<span data-ttu-id="c13f1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c13f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c13f1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c13f1-123">Authorization</span></span>|<span data-ttu-id="c13f1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c13f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c13f1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c13f1-125">Accept</span></span>|<span data-ttu-id="c13f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c13f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c13f1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f1-127">Request body</span></span>
<span data-ttu-id="c13f1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c13f1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c13f1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13f1-129">Response</span></span>
<span data-ttu-id="c13f1-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c13f1-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c13f1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c13f1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c13f1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c13f1-132">Request</span></span>
<span data-ttu-id="c13f1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c13f1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection
```

### <a name="response"></a><span data-ttu-id="c13f1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c13f1-134">Response</span></span>
<span data-ttu-id="c13f1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c13f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
      "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "model": "Model value",
      "virtualNetwork": "Virtual Network value",
      "deviceCount": 11,
      "cloudPcRoundTripTime": 6.666666666666667,
      "cloudPcSignInTime": 5.666666666666667,
      "remoteSignInTime": 5.333333333333333,
      "coreBootTime": 4.0,
      "coreSignInTime": 4.666666666666667,
      "cloudPcFailurePercentage": 8.0
    }
  ]
}
```




