---
title: Obter deviceManagementIntentDeviceSettingStateSummary
description: Leia as propriedades e as relações do objeto deviceManagementIntentDeviceSettingStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4c6f188f4cad19f5f2f705955e2926ea3c61726
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767243"
---
# <a name="get-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="33a38-103">Obter deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="33a38-103">Get deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="33a38-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33a38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33a38-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33a38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33a38-106">Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="33a38-106">Read properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33a38-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33a38-107">Prerequisites</span></span>
<span data-ttu-id="33a38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33a38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a38-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33a38-110">Permission type</span></span>|<span data-ttu-id="33a38-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33a38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33a38-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33a38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33a38-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33a38-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="33a38-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33a38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33a38-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33a38-115">Not supported.</span></span>|
|<span data-ttu-id="33a38-116">Application</span><span class="sxs-lookup"><span data-stu-id="33a38-116">Application</span></span>|<span data-ttu-id="33a38-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33a38-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33a38-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33a38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33a38-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="33a38-119">Optional query parameters</span></span>
<span data-ttu-id="33a38-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="33a38-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33a38-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33a38-121">Request headers</span></span>
|<span data-ttu-id="33a38-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33a38-122">Header</span></span>|<span data-ttu-id="33a38-123">Valor</span><span class="sxs-lookup"><span data-stu-id="33a38-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33a38-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="33a38-124">Authorization</span></span>|<span data-ttu-id="33a38-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33a38-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33a38-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33a38-126">Accept</span></span>|<span data-ttu-id="33a38-127">application/json</span><span class="sxs-lookup"><span data-stu-id="33a38-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33a38-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33a38-128">Request body</span></span>
<span data-ttu-id="33a38-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33a38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33a38-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a38-130">Response</span></span>
<span data-ttu-id="33a38-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33a38-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33a38-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33a38-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="33a38-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33a38-133">Request</span></span>
<span data-ttu-id="33a38-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33a38-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="33a38-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a38-135">Response</span></span>
<span data-ttu-id="33a38-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33a38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




