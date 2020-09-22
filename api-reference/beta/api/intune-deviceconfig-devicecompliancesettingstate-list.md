---
title: Listar deviceComplianceSettingStates
description: Listar propriedades e relações dos objetos deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05628cd87448595883ee0866eb832e3ac7ad3094
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011666"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="79029-103">Listar deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="79029-103">List deviceComplianceSettingStates</span></span>

<span data-ttu-id="79029-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="79029-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79029-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79029-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79029-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79029-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79029-107">Listar propriedades e relações dos objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="79029-107">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79029-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79029-108">Prerequisites</span></span>
<span data-ttu-id="79029-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79029-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79029-111">Permission type</span></span>|<span data-ttu-id="79029-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79029-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79029-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79029-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79029-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79029-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79029-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79029-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79029-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79029-116">Not supported.</span></span>|
|<span data-ttu-id="79029-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79029-117">Application</span></span>|<span data-ttu-id="79029-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79029-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79029-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79029-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="79029-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79029-120">Request headers</span></span>
|<span data-ttu-id="79029-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79029-121">Header</span></span>|<span data-ttu-id="79029-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79029-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79029-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79029-123">Authorization</span></span>|<span data-ttu-id="79029-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79029-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79029-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79029-125">Accept</span></span>|<span data-ttu-id="79029-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79029-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79029-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79029-127">Request body</span></span>
<span data-ttu-id="79029-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79029-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79029-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="79029-129">Response</span></span>
<span data-ttu-id="79029-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79029-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79029-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79029-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="79029-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79029-132">Request</span></span>
<span data-ttu-id="79029-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79029-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="79029-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="79029-134">Response</span></span>
<span data-ttu-id="79029-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79029-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "platformType": "windowsRT",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```






