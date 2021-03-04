---
title: Obter userExperienceAnalyticsRemoteConnection
description: Leia propriedades e relações do objeto userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69eaa9af1cab4e37c6fe5f359e4da0731b2c61d0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445914"
---
# <a name="get-userexperienceanalyticsremoteconnection"></a><span data-ttu-id="da905-103">Obter userExperienceAnalyticsRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="da905-103">Get userExperienceAnalyticsRemoteConnection</span></span>

<span data-ttu-id="da905-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da905-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da905-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da905-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da905-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da905-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da905-107">Leia propriedades e relações do [objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="da905-107">Read properties and relationships of the [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da905-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da905-108">Prerequisites</span></span>
<span data-ttu-id="da905-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da905-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da905-111">Permission type</span></span>|<span data-ttu-id="da905-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da905-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da905-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da905-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da905-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="da905-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="da905-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da905-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da905-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da905-116">Not supported.</span></span>|
|<span data-ttu-id="da905-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da905-117">Application</span></span>|<span data-ttu-id="da905-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="da905-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da905-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da905-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da905-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da905-120">Optional query parameters</span></span>
<span data-ttu-id="da905-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da905-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da905-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da905-122">Request headers</span></span>
|<span data-ttu-id="da905-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da905-123">Header</span></span>|<span data-ttu-id="da905-124">Valor</span><span class="sxs-lookup"><span data-stu-id="da905-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da905-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="da905-125">Authorization</span></span>|<span data-ttu-id="da905-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da905-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da905-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da905-127">Accept</span></span>|<span data-ttu-id="da905-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da905-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da905-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da905-129">Request body</span></span>
<span data-ttu-id="da905-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da905-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da905-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="da905-131">Response</span></span>
<span data-ttu-id="da905-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da905-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da905-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da905-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="da905-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da905-134">Request</span></span>
<span data-ttu-id="da905-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da905-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

### <a name="response"></a><span data-ttu-id="da905-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="da905-136">Response</span></span>
<span data-ttu-id="da905-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da905-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 573

{
  "value": {
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
}
```




