---
title: Listar deviceManagementIntentDeviceSettingStateSummaries
description: Listar Propriedades e relações dos objetos deviceManagementIntentDeviceSettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52382173b6982a76948d9fef86239c7111e52c7c
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522360"
---
# <a name="list-devicemanagementintentdevicesettingstatesummaries"></a><span data-ttu-id="52c44-103">Listar deviceManagementIntentDeviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="52c44-103">List deviceManagementIntentDeviceSettingStateSummaries</span></span>

> <span data-ttu-id="52c44-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52c44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52c44-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52c44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52c44-106">Listar Propriedades e relações dos objetos [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="52c44-106">List properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52c44-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52c44-107">Prerequisites</span></span>
<span data-ttu-id="52c44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52c44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52c44-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52c44-110">Permission type</span></span>|<span data-ttu-id="52c44-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52c44-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52c44-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52c44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52c44-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52c44-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="52c44-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52c44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52c44-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52c44-115">Not supported.</span></span>|
|<span data-ttu-id="52c44-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52c44-116">Application</span></span>|<span data-ttu-id="52c44-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52c44-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52c44-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52c44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="52c44-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52c44-119">Request headers</span></span>
|<span data-ttu-id="52c44-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52c44-120">Header</span></span>|<span data-ttu-id="52c44-121">Valor</span><span class="sxs-lookup"><span data-stu-id="52c44-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52c44-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="52c44-122">Authorization</span></span>|<span data-ttu-id="52c44-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52c44-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52c44-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52c44-124">Accept</span></span>|<span data-ttu-id="52c44-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52c44-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52c44-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52c44-126">Request body</span></span>
<span data-ttu-id="52c44-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52c44-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52c44-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="52c44-128">Response</span></span>
<span data-ttu-id="52c44-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52c44-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52c44-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52c44-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="52c44-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52c44-131">Request</span></span>
<span data-ttu-id="52c44-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52c44-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="52c44-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="52c44-133">Response</span></span>
<span data-ttu-id="52c44-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52c44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "value": [
    {
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
  ]
}
```







