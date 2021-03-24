---
title: Listar advancedThreatProtectionOnboardingDeviceSettingStates
description: Listar propriedades e relações dos objetos advancedThreatProtectionOnboardingDeviceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f19e5b5b99ee9555d4f5dbc84fe9ede16e87191
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126889"
---
# <a name="list-advancedthreatprotectiononboardingdevicesettingstates"></a><span data-ttu-id="b3322-103">Listar advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="b3322-103">List advancedThreatProtectionOnboardingDeviceSettingStates</span></span>

<span data-ttu-id="b3322-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3322-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3322-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3322-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3322-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3322-107">Listar propriedades e relações dos [objetos advancedThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="b3322-107">List properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3322-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3322-108">Prerequisites</span></span>
<span data-ttu-id="b3322-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3322-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3322-111">Permission type</span></span>|<span data-ttu-id="b3322-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3322-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3322-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3322-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3322-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3322-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3322-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3322-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3322-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3322-116">Not supported.</span></span>|
|<span data-ttu-id="b3322-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3322-117">Application</span></span>|<span data-ttu-id="b3322-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3322-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3322-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3322-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="b3322-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3322-120">Request headers</span></span>
|<span data-ttu-id="b3322-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3322-121">Header</span></span>|<span data-ttu-id="b3322-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3322-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3322-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3322-123">Authorization</span></span>|<span data-ttu-id="b3322-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3322-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3322-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3322-125">Accept</span></span>|<span data-ttu-id="b3322-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3322-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3322-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3322-127">Request body</span></span>
<span data-ttu-id="b3322-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3322-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3322-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3322-129">Response</span></span>
<span data-ttu-id="b3322-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3322-130">If successful, this method returns a `200 OK` response code and a collection of [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3322-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3322-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3322-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3322-132">Request</span></span>
<span data-ttu-id="b3322-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3322-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

### <a name="response"></a><span data-ttu-id="b3322-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3322-134">Response</span></span>
<span data-ttu-id="b3322-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3322-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




