---
title: Obter advancedThreatProtectionOnboardingDeviceSettingState
description: Leia as propriedades e os relacionamentos do objeto advancedThreatProtectionOnboardingDeviceSettingState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6600447ba7a61342d7d05d54f3a6a405b396bb76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409577"
---
# <a name="get-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="5275e-103">Obter advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="5275e-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="5275e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5275e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5275e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5275e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5275e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5275e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5275e-107">Leia as propriedades e os relacionamentos do objeto [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5275e-107">Read properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5275e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5275e-108">Prerequisites</span></span>
<span data-ttu-id="5275e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5275e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5275e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5275e-111">Permission type</span></span>|<span data-ttu-id="5275e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5275e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5275e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5275e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5275e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5275e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5275e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5275e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5275e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5275e-116">Not supported.</span></span>|
|<span data-ttu-id="5275e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5275e-117">Application</span></span>|<span data-ttu-id="5275e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5275e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5275e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5275e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5275e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5275e-120">Optional query parameters</span></span>
<span data-ttu-id="5275e-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5275e-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5275e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5275e-122">Request headers</span></span>
|<span data-ttu-id="5275e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5275e-123">Header</span></span>|<span data-ttu-id="5275e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5275e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5275e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5275e-125">Authorization</span></span>|<span data-ttu-id="5275e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5275e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5275e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5275e-127">Accept</span></span>|<span data-ttu-id="5275e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5275e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5275e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5275e-129">Request body</span></span>
<span data-ttu-id="5275e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5275e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5275e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5275e-131">Response</span></span>
<span data-ttu-id="5275e-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5275e-132">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5275e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5275e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5275e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5275e-134">Request</span></span>
<span data-ttu-id="5275e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5275e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="5275e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5275e-136">Response</span></span>
<span data-ttu-id="5275e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5275e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 669

{
  "value": {
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
}
```




