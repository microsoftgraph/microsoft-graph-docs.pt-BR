---
title: Obter androidForWorkGeneralDeviceConfiguration
description: Leia as propriedades e as relações do objeto androidForWorkGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 488f029b59838c2f33d24a0708337573e20d4139
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957868"
---
# <a name="get-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="87cc2-103">Obter androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="87cc2-103">Get androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="87cc2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87cc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87cc2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87cc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87cc2-106">Leia as propriedades e as relações do objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="87cc2-106">Read properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87cc2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87cc2-107">Prerequisites</span></span>
<span data-ttu-id="87cc2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87cc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87cc2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87cc2-110">Permission type</span></span>|<span data-ttu-id="87cc2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87cc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87cc2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87cc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87cc2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87cc2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87cc2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87cc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87cc2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87cc2-115">Not supported.</span></span>|
|<span data-ttu-id="87cc2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87cc2-116">Application</span></span>|<span data-ttu-id="87cc2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87cc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87cc2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87cc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87cc2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87cc2-119">Optional query parameters</span></span>
<span data-ttu-id="87cc2-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87cc2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87cc2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87cc2-121">Request headers</span></span>
|<span data-ttu-id="87cc2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87cc2-122">Header</span></span>|<span data-ttu-id="87cc2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="87cc2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87cc2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="87cc2-124">Authorization</span></span>|<span data-ttu-id="87cc2-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87cc2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87cc2-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87cc2-126">Accept</span></span>|<span data-ttu-id="87cc2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="87cc2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87cc2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87cc2-128">Request body</span></span>
<span data-ttu-id="87cc2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87cc2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87cc2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="87cc2-130">Response</span></span>
<span data-ttu-id="87cc2-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87cc2-131">If successful, this method returns a `200 OK` response code and [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87cc2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87cc2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="87cc2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87cc2-133">Request</span></span>
<span data-ttu-id="87cc2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87cc2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="87cc2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="87cc2-135">Response</span></span>
<span data-ttu-id="87cc2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87cc2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2323

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
    "id": "a931a366-a366-a931-66a3-31a966a331a9",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "lowSecurityBiometric",
    "workProfileDataSharingType": "preventAny",
    "workProfileBlockNotificationsWhileDeviceLocked": true,
    "workProfileBlockAddingAccounts": true,
    "workProfileBluetoothEnableContactSharing": true,
    "workProfileBlockScreenCapture": true,
    "workProfileBlockCrossProfileCallerId": true,
    "workProfileBlockCamera": true,
    "workProfileBlockCrossProfileContactsSearch": true,
    "workProfileBlockCrossProfileCopyPaste": true,
    "workProfileDefaultAppPermissionPolicy": "prompt",
    "workProfilePasswordBlockFingerprintUnlock": true,
    "workProfilePasswordBlockTrustAgents": true,
    "workProfilePasswordExpirationDays": 1,
    "workProfilePasswordMinimumLength": 0,
    "workProfilePasswordMinNumericCharacters": 7,
    "workProfilePasswordMinNonLetterCharacters": 9,
    "workProfilePasswordMinLetterCharacters": 6,
    "workProfilePasswordMinLowerCaseCharacters": 9,
    "workProfilePasswordMinUpperCaseCharacters": 9,
    "workProfilePasswordMinSymbolCharacters": 6,
    "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
    "workProfilePasswordPreviousPasswordBlockCount": 13,
    "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
    "workProfilePasswordRequiredType": "lowSecurityBiometric",
    "workProfileRequirePassword": true,
    "securityRequireVerifyApps": true,
    "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
    "vpnEnableAlwaysOnLockdownMode": true
  }
}
```




