---
title: Lista advancedThreatProtectionOnboardingDeviceSettingStates
description: Lista as propriedades e os relacionamentos dos objetos advancedThreatProtectionOnboardingDeviceSettingState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4ac88f85cd6095644aefb303ff111649aa48aa8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395073"
---
# <a name="list-advancedthreatprotectiononboardingdevicesettingstates"></a><span data-ttu-id="038ec-103">Lista advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="038ec-103">List advancedThreatProtectionOnboardingDeviceSettingStates</span></span>

> <span data-ttu-id="038ec-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="038ec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="038ec-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="038ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="038ec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="038ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="038ec-107">Lista as propriedades e os relacionamentos dos objetos [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="038ec-107">List properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="038ec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="038ec-108">Prerequisites</span></span>
<span data-ttu-id="038ec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="038ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="038ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="038ec-111">Permission type</span></span>|<span data-ttu-id="038ec-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="038ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="038ec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="038ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="038ec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="038ec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="038ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="038ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="038ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="038ec-116">Not supported.</span></span>|
|<span data-ttu-id="038ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="038ec-117">Application</span></span>|<span data-ttu-id="038ec-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="038ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="038ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="038ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="038ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="038ec-120">Request headers</span></span>
|<span data-ttu-id="038ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="038ec-121">Header</span></span>|<span data-ttu-id="038ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="038ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="038ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="038ec-123">Authorization</span></span>|<span data-ttu-id="038ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="038ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="038ec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="038ec-125">Accept</span></span>|<span data-ttu-id="038ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="038ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="038ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="038ec-127">Request body</span></span>
<span data-ttu-id="038ec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="038ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="038ec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="038ec-129">Response</span></span>
<span data-ttu-id="038ec-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="038ec-130">If successful, this method returns a `200 OK` response code and a collection of [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="038ec-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="038ec-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="038ec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="038ec-132">Request</span></span>
<span data-ttu-id="038ec-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="038ec-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

### <a name="response"></a><span data-ttu-id="038ec-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="038ec-134">Response</span></span>
<span data-ttu-id="038ec-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="038ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




