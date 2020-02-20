---
title: Obter userExperienceAnalyticsDeviceStartupProcess
description: Leia as propriedades e as relações do objeto userExperienceAnalyticsDeviceStartupProcess.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2b75490562c595c83d7fdaaa204d7bc3c79bfd06
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161991"
---
# <a name="get-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="d2689-103">Obter userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="d2689-103">Get userExperienceAnalyticsDeviceStartupProcess</span></span>

> <span data-ttu-id="d2689-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2689-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2689-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2689-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2689-106">Leia as propriedades e as relações do objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="d2689-106">Read properties and relationships of the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2689-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2689-107">Prerequisites</span></span>
<span data-ttu-id="d2689-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2689-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2689-110">Permission type</span></span>|<span data-ttu-id="d2689-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2689-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2689-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2689-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2689-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2689-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d2689-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2689-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2689-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2689-115">Not supported.</span></span>|
|<span data-ttu-id="d2689-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2689-116">Application</span></span>|<span data-ttu-id="d2689-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2689-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2689-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2689-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2689-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2689-119">Optional query parameters</span></span>
<span data-ttu-id="d2689-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2689-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2689-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2689-121">Request headers</span></span>
|<span data-ttu-id="d2689-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2689-122">Header</span></span>|<span data-ttu-id="d2689-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d2689-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2689-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2689-124">Authorization</span></span>|<span data-ttu-id="d2689-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2689-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2689-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2689-126">Accept</span></span>|<span data-ttu-id="d2689-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d2689-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2689-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2689-128">Request body</span></span>
<span data-ttu-id="d2689-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2689-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2689-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2689-130">Response</span></span>
<span data-ttu-id="d2689-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2689-131">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2689-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2689-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2689-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2689-133">Request</span></span>
<span data-ttu-id="d2689-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2689-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

### <a name="response"></a><span data-ttu-id="d2689-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2689-135">Response</span></span>
<span data-ttu-id="d2689-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2689-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





