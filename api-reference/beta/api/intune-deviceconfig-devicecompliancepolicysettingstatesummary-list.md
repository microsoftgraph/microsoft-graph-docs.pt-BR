---
title: Listar deviceCompliancePolicySettingStateSummaries
description: Listar propriedades e relações dos objetos deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 145862c60e423f03b44ffa1e9d4722d8750995bb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433918"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="6b97f-103">Listar deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="6b97f-103">List deviceCompliancePolicySettingStateSummaries</span></span>

<span data-ttu-id="6b97f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b97f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b97f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b97f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b97f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b97f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b97f-107">Listar propriedades e relações dos objetos [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b97f-107">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b97f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b97f-108">Prerequisites</span></span>
<span data-ttu-id="6b97f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b97f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b97f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b97f-111">Permission type</span></span>|<span data-ttu-id="6b97f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b97f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b97f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b97f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b97f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b97f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6b97f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b97f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b97f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b97f-116">Not supported.</span></span>|
|<span data-ttu-id="6b97f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b97f-117">Application</span></span>|<span data-ttu-id="6b97f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b97f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b97f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b97f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="6b97f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b97f-120">Request headers</span></span>
|<span data-ttu-id="6b97f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b97f-121">Header</span></span>|<span data-ttu-id="6b97f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b97f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b97f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b97f-123">Authorization</span></span>|<span data-ttu-id="6b97f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b97f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b97f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b97f-125">Accept</span></span>|<span data-ttu-id="6b97f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b97f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b97f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b97f-127">Request body</span></span>
<span data-ttu-id="6b97f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b97f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b97f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b97f-129">Response</span></span>
<span data-ttu-id="6b97f-130">Se tiver êxito, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b97f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b97f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b97f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b97f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b97f-132">Request</span></span>
<span data-ttu-id="6b97f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b97f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="6b97f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b97f-134">Response</span></span>
<span data-ttu-id="6b97f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b97f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



