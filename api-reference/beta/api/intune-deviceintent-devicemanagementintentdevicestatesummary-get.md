---
title: Obter deviceManagementIntentDeviceStateSummary
description: Leia as propriedades e as relações do objeto deviceManagementIntentDeviceStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29e3b3bb50039eabb78efd43a65f5844eb5ee59e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087731"
---
# <a name="get-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="6c2ba-103">Obter deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="6c2ba-103">Get deviceManagementIntentDeviceStateSummary</span></span>

> <span data-ttu-id="6c2ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c2ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c2ba-106">Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="6c2ba-106">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c2ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c2ba-107">Prerequisites</span></span>
<span data-ttu-id="6c2ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c2ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c2ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c2ba-110">Permission type</span></span>|<span data-ttu-id="6c2ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c2ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c2ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c2ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c2ba-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c2ba-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6c2ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c2ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c2ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-115">Not supported.</span></span>|
|<span data-ttu-id="6c2ba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c2ba-116">Application</span></span>|<span data-ttu-id="6c2ba-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c2ba-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c2ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c2ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c2ba-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c2ba-119">Optional query parameters</span></span>
<span data-ttu-id="6c2ba-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c2ba-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2ba-121">Request headers</span></span>
|<span data-ttu-id="6c2ba-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c2ba-122">Header</span></span>|<span data-ttu-id="6c2ba-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6c2ba-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c2ba-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c2ba-124">Authorization</span></span>|<span data-ttu-id="6c2ba-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c2ba-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c2ba-126">Accept</span></span>|<span data-ttu-id="6c2ba-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c2ba-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c2ba-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2ba-128">Request body</span></span>
<span data-ttu-id="6c2ba-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c2ba-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c2ba-130">Response</span></span>
<span data-ttu-id="6c2ba-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c2ba-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c2ba-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c2ba-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2ba-133">Request</span></span>
<span data-ttu-id="6c2ba-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

### <a name="response"></a><span data-ttu-id="6c2ba-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c2ba-135">Response</span></span>
<span data-ttu-id="6c2ba-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c2ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 321

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
    "id": "12230bf9-0bf9-1223-f90b-2312f90b2312",
    "conflictCount": 13,
    "errorCount": 10,
    "failedCount": 11,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12
  }
}
```






