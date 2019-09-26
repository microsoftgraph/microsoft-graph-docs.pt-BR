---
title: Obter deviceManagementIntentDeviceSettingStateSummary
description: Leia as propriedades e as relações do objeto deviceManagementIntentDeviceSettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c842dba90ae455e54293bcfa379217aa70f8d315
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185872"
---
# <a name="get-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="e78ab-103">Obter deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="e78ab-103">Get deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="e78ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e78ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e78ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e78ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e78ab-106">Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e78ab-106">Read properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e78ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e78ab-107">Prerequisites</span></span>
<span data-ttu-id="e78ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e78ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e78ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e78ab-110">Permission type</span></span>|<span data-ttu-id="e78ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e78ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e78ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e78ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e78ab-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e78ab-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e78ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e78ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e78ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e78ab-115">Not supported.</span></span>|
|<span data-ttu-id="e78ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e78ab-116">Application</span></span>|<span data-ttu-id="e78ab-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e78ab-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e78ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e78ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e78ab-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e78ab-119">Optional query parameters</span></span>
<span data-ttu-id="e78ab-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e78ab-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e78ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e78ab-121">Request headers</span></span>
|<span data-ttu-id="e78ab-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e78ab-122">Header</span></span>|<span data-ttu-id="e78ab-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e78ab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e78ab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e78ab-124">Authorization</span></span>|<span data-ttu-id="e78ab-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e78ab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e78ab-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e78ab-126">Accept</span></span>|<span data-ttu-id="e78ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e78ab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e78ab-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e78ab-128">Request body</span></span>
<span data-ttu-id="e78ab-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e78ab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e78ab-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78ab-130">Response</span></span>
<span data-ttu-id="e78ab-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e78ab-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e78ab-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e78ab-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e78ab-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e78ab-133">Request</span></span>
<span data-ttu-id="e78ab-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e78ab-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="e78ab-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78ab-135">Response</span></span>
<span data-ttu-id="e78ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e78ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 366

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
    "id": "d3d3a75f-a75f-d3d3-5fa7-d3d35fa7d3d3",
    "settingName": "Setting Name value",
    "compliantCount": 14,
    "conflictCount": 13,
    "errorCount": 10,
    "nonCompliantCount": 1,
    "notApplicableCount": 2,
    "remediatedCount": 15
  }
}
```




