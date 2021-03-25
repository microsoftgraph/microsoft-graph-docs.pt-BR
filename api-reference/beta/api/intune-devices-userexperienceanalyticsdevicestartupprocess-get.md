---
title: Obter userExperienceAnalyticsDeviceStartupProcess
description: Leia propriedades e relações do objeto userExperienceAnalyticsDeviceStartupProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc0cd0e174add6eac798dfa1ca2705771aca85e8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154088"
---
# <a name="get-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="57c4f-103">Obter userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="57c4f-103">Get userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="57c4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57c4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57c4f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57c4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57c4f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57c4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57c4f-107">Leia propriedades e relações do [objeto userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)</span><span class="sxs-lookup"><span data-stu-id="57c4f-107">Read properties and relationships of the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57c4f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57c4f-108">Prerequisites</span></span>
<span data-ttu-id="57c4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57c4f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57c4f-111">Permission type</span></span>|<span data-ttu-id="57c4f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57c4f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57c4f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57c4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57c4f-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57c4f-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57c4f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57c4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57c4f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57c4f-116">Not supported.</span></span>|
|<span data-ttu-id="57c4f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57c4f-117">Application</span></span>|<span data-ttu-id="57c4f-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57c4f-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57c4f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57c4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57c4f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="57c4f-120">Optional query parameters</span></span>
<span data-ttu-id="57c4f-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57c4f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57c4f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57c4f-122">Request headers</span></span>
|<span data-ttu-id="57c4f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57c4f-123">Header</span></span>|<span data-ttu-id="57c4f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="57c4f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57c4f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="57c4f-125">Authorization</span></span>|<span data-ttu-id="57c4f-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57c4f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57c4f-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57c4f-127">Accept</span></span>|<span data-ttu-id="57c4f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="57c4f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57c4f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57c4f-129">Request body</span></span>
<span data-ttu-id="57c4f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57c4f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57c4f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="57c4f-131">Response</span></span>
<span data-ttu-id="57c4f-132">Se tiver êxito, este método retornará um código de resposta e o `200 OK` [objeto userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57c4f-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57c4f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57c4f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="57c4f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57c4f-134">Request</span></span>
<span data-ttu-id="57c4f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57c4f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

### <a name="response"></a><span data-ttu-id="57c4f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="57c4f-136">Response</span></span>
<span data-ttu-id="57c4f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57c4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
    "id": "03b451e6-51e6-03b4-e651-b403e651b403",
    "managedDeviceId": "Managed Device Id value",
    "processName": "Process Name value",
    "productName": "Product Name value",
    "publisher": "Publisher value",
    "startupImpactInMs": 1
  }
}
```




