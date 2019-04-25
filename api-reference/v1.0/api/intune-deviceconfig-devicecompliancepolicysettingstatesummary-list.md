---
title: Listar deviceCompliancePolicySettingStateSummaries
description: Listar propriedades e relações dos objetos deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29f64028604c3f3402c12d4b08170f5925d1cd8e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580824"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="d9d45-103">Listar deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="d9d45-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="d9d45-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9d45-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9d45-105">Listar propriedades e relações dos objetos [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d9d45-105">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9d45-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9d45-106">Prerequisites</span></span>
<span data-ttu-id="d9d45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9d45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9d45-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9d45-109">Permission type</span></span>|<span data-ttu-id="d9d45-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9d45-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9d45-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9d45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9d45-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9d45-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d9d45-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9d45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9d45-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9d45-114">Not supported.</span></span>|
|<span data-ttu-id="d9d45-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9d45-115">Application</span></span>|<span data-ttu-id="d9d45-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9d45-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9d45-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d45-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d9d45-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d45-118">Request headers</span></span>
|<span data-ttu-id="d9d45-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9d45-119">Header</span></span>|<span data-ttu-id="d9d45-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d9d45-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9d45-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9d45-121">Authorization</span></span>|<span data-ttu-id="d9d45-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9d45-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9d45-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9d45-123">Accept</span></span>|<span data-ttu-id="d9d45-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d9d45-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9d45-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d45-125">Request body</span></span>
<span data-ttu-id="d9d45-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9d45-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9d45-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d45-127">Response</span></span>
<span data-ttu-id="d9d45-128">Se tiver êxito, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9d45-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9d45-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9d45-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9d45-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d45-130">Request</span></span>
<span data-ttu-id="d9d45-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9d45-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="d9d45-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d45-132">Response</span></span>
<span data-ttu-id="d9d45-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9d45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
      "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "platformType": "iOS",
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



