---
title: Lista androidForWorkGeneralDeviceConfigurations
description: Lista as propriedades e os relacionamentos dos objetos androidForWorkGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 44880be8c782697e0eb84743fb3fb249235ac2d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933705"
---
# <a name="list-androidforworkgeneraldeviceconfigurations"></a><span data-ttu-id="69b30-103">Lista androidForWorkGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="69b30-103">List androidForWorkGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="69b30-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="69b30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69b30-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="69b30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69b30-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="69b30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69b30-107">Lista as propriedades e os relacionamentos dos objetos [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="69b30-107">List properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69b30-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69b30-108">Prerequisites</span></span>
<span data-ttu-id="69b30-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69b30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69b30-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69b30-111">Permission type</span></span>|<span data-ttu-id="69b30-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69b30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69b30-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69b30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69b30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69b30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="69b30-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69b30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69b30-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69b30-116">Not supported.</span></span>|
|<span data-ttu-id="69b30-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69b30-117">Application</span></span>|<span data-ttu-id="69b30-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69b30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69b30-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69b30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="69b30-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69b30-120">Request headers</span></span>
|<span data-ttu-id="69b30-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69b30-121">Header</span></span>|<span data-ttu-id="69b30-122">Valor</span><span class="sxs-lookup"><span data-stu-id="69b30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69b30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="69b30-123">Authorization</span></span>|<span data-ttu-id="69b30-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69b30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69b30-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69b30-125">Accept</span></span>|<span data-ttu-id="69b30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69b30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69b30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69b30-127">Request body</span></span>
<span data-ttu-id="69b30-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69b30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69b30-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="69b30-129">Response</span></span>
<span data-ttu-id="69b30-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69b30-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69b30-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69b30-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="69b30-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69b30-132">Request</span></span>
<span data-ttu-id="69b30-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69b30-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="69b30-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="69b30-134">Response</span></span>
<span data-ttu-id="69b30-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69b30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2431

{
  "value": [
    {
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
  ]
}
```





