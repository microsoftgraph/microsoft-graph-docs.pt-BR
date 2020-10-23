---
title: Listar advancedThreatProtectionOnboardingDeviceSettingStates
description: Listar Propriedades e relações dos objetos advancedThreatProtectionOnboardingDeviceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 971187957555697e4dd3e35836120c78e8a8c994
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698943"
---
# <a name="list-advancedthreatprotectiononboardingdevicesettingstates"></a><span data-ttu-id="80ee8-103">Listar advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="80ee8-103">List advancedThreatProtectionOnboardingDeviceSettingStates</span></span>

<span data-ttu-id="80ee8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80ee8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80ee8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80ee8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80ee8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80ee8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80ee8-107">Listar Propriedades e relações dos objetos [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="80ee8-107">List properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80ee8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80ee8-108">Prerequisites</span></span>
<span data-ttu-id="80ee8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80ee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80ee8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80ee8-111">Permission type</span></span>|<span data-ttu-id="80ee8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80ee8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80ee8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80ee8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80ee8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="80ee8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="80ee8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80ee8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80ee8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80ee8-116">Not supported.</span></span>|
|<span data-ttu-id="80ee8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80ee8-117">Application</span></span>|<span data-ttu-id="80ee8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="80ee8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80ee8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80ee8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="80ee8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80ee8-120">Request headers</span></span>
|<span data-ttu-id="80ee8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80ee8-121">Header</span></span>|<span data-ttu-id="80ee8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="80ee8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80ee8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="80ee8-123">Authorization</span></span>|<span data-ttu-id="80ee8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80ee8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80ee8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80ee8-125">Accept</span></span>|<span data-ttu-id="80ee8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80ee8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80ee8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80ee8-127">Request body</span></span>
<span data-ttu-id="80ee8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80ee8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80ee8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ee8-129">Response</span></span>
<span data-ttu-id="80ee8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80ee8-130">If successful, this method returns a `200 OK` response code and a collection of [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80ee8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80ee8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="80ee8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80ee8-132">Request</span></span>
<span data-ttu-id="80ee8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80ee8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

### <a name="response"></a><span data-ttu-id="80ee8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ee8-134">Response</span></span>
<span data-ttu-id="80ee8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80ee8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 711

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
      "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
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





