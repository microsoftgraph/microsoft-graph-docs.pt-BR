---
title: Obter userExperienceAnalyticsNotAutopilotReadyDevice
description: Leia propriedades e relações do objeto userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11f62ae385e19748fa91f3ef90b32e69e2f5fbe7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867039"
---
# <a name="get-userexperienceanalyticsnotautopilotreadydevice"></a><span data-ttu-id="b0cd3-103">Obter userExperienceAnalyticsNotAutopilotReadyDevice</span><span class="sxs-lookup"><span data-stu-id="b0cd3-103">Get userExperienceAnalyticsNotAutopilotReadyDevice</span></span>

<span data-ttu-id="b0cd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0cd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0cd3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0cd3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0cd3-107">Leia propriedades e relações do [objeto userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="b0cd3-107">Read properties and relationships of the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0cd3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0cd3-108">Prerequisites</span></span>
<span data-ttu-id="b0cd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0cd3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0cd3-111">Permission type</span></span>|<span data-ttu-id="b0cd3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0cd3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0cd3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0cd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0cd3-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0cd3-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b0cd3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0cd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0cd3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-116">Not supported.</span></span>|
|<span data-ttu-id="b0cd3-117">Application</span><span class="sxs-lookup"><span data-stu-id="b0cd3-117">Application</span></span>|<span data-ttu-id="b0cd3-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0cd3-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0cd3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0cd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice/{userExperienceAnalyticsNotAutopilotReadyDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0cd3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0cd3-120">Optional query parameters</span></span>
<span data-ttu-id="b0cd3-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0cd3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0cd3-122">Request headers</span></span>
|<span data-ttu-id="b0cd3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0cd3-123">Header</span></span>|<span data-ttu-id="b0cd3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b0cd3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0cd3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0cd3-125">Authorization</span></span>|<span data-ttu-id="b0cd3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0cd3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0cd3-127">Accept</span></span>|<span data-ttu-id="b0cd3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b0cd3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0cd3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0cd3-129">Request body</span></span>
<span data-ttu-id="b0cd3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0cd3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0cd3-131">Response</span></span>
<span data-ttu-id="b0cd3-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0cd3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0cd3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0cd3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0cd3-134">Request</span></span>
<span data-ttu-id="b0cd3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice/{userExperienceAnalyticsNotAutopilotReadyDeviceId}
```

### <a name="response"></a><span data-ttu-id="b0cd3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0cd3-136">Response</span></span>
<span data-ttu-id="b0cd3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0cd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
    "id": "11c3ffd7-ffd7-11c3-d7ff-c311d7ffc311",
    "deviceName": "Device Name value",
    "serialNumber": "Serial Number value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "managedBy": "Managed By value",
    "autoPilotRegistered": true,
    "autoPilotProfileAssigned": true,
    "azureAdRegistered": true,
    "azureAdJoinType": "Azure Ad Join Type value"
  }
}
```




