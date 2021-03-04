---
title: Obter userExperienceAnalyticsImpactingProcess
description: Leia propriedades e relações do objeto userExperienceAnalyticsImpactingProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b17aee1973d2775794d739221ef89611aee5a0a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445705"
---
# <a name="get-userexperienceanalyticsimpactingprocess"></a><span data-ttu-id="bec93-103">Obter userExperienceAnalyticsImpactingProcess</span><span class="sxs-lookup"><span data-stu-id="bec93-103">Get userExperienceAnalyticsImpactingProcess</span></span>

<span data-ttu-id="bec93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bec93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bec93-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bec93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bec93-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bec93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bec93-107">Leia propriedades e relações do [objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="bec93-107">Read properties and relationships of the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bec93-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bec93-108">Prerequisites</span></span>
<span data-ttu-id="bec93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bec93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bec93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bec93-111">Permission type</span></span>|<span data-ttu-id="bec93-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bec93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bec93-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bec93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bec93-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bec93-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bec93-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bec93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bec93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bec93-116">Not supported.</span></span>|
|<span data-ttu-id="bec93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bec93-117">Application</span></span>|<span data-ttu-id="bec93-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bec93-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bec93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bec93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bec93-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bec93-120">Optional query parameters</span></span>
<span data-ttu-id="bec93-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bec93-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bec93-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bec93-122">Request headers</span></span>
|<span data-ttu-id="bec93-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bec93-123">Header</span></span>|<span data-ttu-id="bec93-124">Valor</span><span class="sxs-lookup"><span data-stu-id="bec93-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bec93-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bec93-125">Authorization</span></span>|<span data-ttu-id="bec93-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bec93-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bec93-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bec93-127">Accept</span></span>|<span data-ttu-id="bec93-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bec93-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bec93-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bec93-129">Request body</span></span>
<span data-ttu-id="bec93-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bec93-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bec93-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bec93-131">Response</span></span>
<span data-ttu-id="bec93-132">Se tiver êxito, este método retornará um código de resposta e o `200 OK` [objeto userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bec93-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bec93-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bec93-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bec93-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bec93-134">Request</span></span>
<span data-ttu-id="bec93-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bec93-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

### <a name="response"></a><span data-ttu-id="bec93-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bec93-136">Response</span></span>
<span data-ttu-id="bec93-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bec93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
    "id": "faefd665-d665-faef-65d6-effa65d6effa",
    "deviceId": "Device Id value",
    "category": "Category value",
    "processName": "Process Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "impactValue": 3.6666666666666665
  }
}
```




