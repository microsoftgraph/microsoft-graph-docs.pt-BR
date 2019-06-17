---
title: Listar deviceCompliancePolicySettingStateSummaries
description: Listar propriedades e relações dos objetos deviceCompliancePolicySettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df0e0fbeaccc0aa0a96a63fe518cd369354e1847
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968291"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="a6ceb-103">Listar deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a6ceb-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="a6ceb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6ceb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6ceb-106">Listar propriedades e relações dos objetos [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a6ceb-106">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6ceb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6ceb-107">Prerequisites</span></span>
<span data-ttu-id="a6ceb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6ceb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6ceb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6ceb-110">Permission type</span></span>|<span data-ttu-id="a6ceb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6ceb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6ceb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6ceb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6ceb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6ceb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a6ceb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6ceb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6ceb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-115">Not supported.</span></span>|
|<span data-ttu-id="a6ceb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6ceb-116">Application</span></span>|<span data-ttu-id="a6ceb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6ceb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6ceb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a6ceb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ceb-119">Request headers</span></span>
|<span data-ttu-id="a6ceb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6ceb-120">Header</span></span>|<span data-ttu-id="a6ceb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a6ceb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6ceb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6ceb-122">Authorization</span></span>|<span data-ttu-id="a6ceb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6ceb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6ceb-124">Accept</span></span>|<span data-ttu-id="a6ceb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6ceb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6ceb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ceb-126">Request body</span></span>
<span data-ttu-id="a6ceb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6ceb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ceb-128">Response</span></span>
<span data-ttu-id="a6ceb-129">Se tiver êxito, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6ceb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6ceb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6ceb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ceb-131">Request</span></span>
<span data-ttu-id="a6ceb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="a6ceb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ceb-133">Response</span></span>
<span data-ttu-id="a6ceb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6ceb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
      "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "platformType": "androidForWork",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```





