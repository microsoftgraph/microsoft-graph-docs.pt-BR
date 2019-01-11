---
title: Lista androidDeviceOwnerGeneralDeviceConfigurations
description: Lista as propriedades e os relacionamentos dos objetos androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c45dac2aea007b2c9b54828376d8ae0b519fd736
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838567"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a><span data-ttu-id="45bb1-103">Lista androidDeviceOwnerGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="45bb1-103">List androidDeviceOwnerGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="45bb1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="45bb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45bb1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45bb1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45bb1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="45bb1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45bb1-107">Lista as propriedades e os relacionamentos dos objetos [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45bb1-107">List properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45bb1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45bb1-108">Prerequisites</span></span>
<span data-ttu-id="45bb1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45bb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45bb1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45bb1-111">Permission type</span></span>|<span data-ttu-id="45bb1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45bb1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45bb1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45bb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45bb1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45bb1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45bb1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45bb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45bb1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45bb1-116">Not supported.</span></span>|
|<span data-ttu-id="45bb1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45bb1-117">Application</span></span>|<span data-ttu-id="45bb1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45bb1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45bb1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45bb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45bb1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45bb1-120">Request headers</span></span>
|<span data-ttu-id="45bb1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45bb1-121">Header</span></span>|<span data-ttu-id="45bb1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45bb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45bb1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45bb1-123">Authorization</span></span>|<span data-ttu-id="45bb1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45bb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45bb1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45bb1-125">Accept</span></span>|<span data-ttu-id="45bb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45bb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45bb1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45bb1-127">Request body</span></span>
<span data-ttu-id="45bb1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45bb1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45bb1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="45bb1-129">Response</span></span>
<span data-ttu-id="45bb1-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45bb1-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45bb1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45bb1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="45bb1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45bb1-132">Request</span></span>
<span data-ttu-id="45bb1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45bb1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="45bb1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="45bb1-134">Response</span></span>
<span data-ttu-id="45bb1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45bb1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2549

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
      "id": "edad943d-943d-edad-3d94-aded3d94aded",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountsBlockModification": true,
      "appsAllowInstallFromUnknownSources": true,
      "appsAutoUpdatePolicy": "userChoice",
      "appsDefaultPermissionPolicy": "prompt",
      "bluetoothBlockConfiguration": true,
      "bluetoothBlockContactSharing": true,
      "cameraBlocked": true,
      "cellularBlockWiFiTethering": true,
      "dataRoamingBlocked": true,
      "dateTimeConfigurationBlocked": true,
      "factoryResetDeviceAdministratorEmails": [
        "Factory Reset Device Administrator Emails value"
      ],
      "factoryResetBlocked": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "microphoneForceMute": true,
      "networkEscapeHatchAllowed": true,
      "nfcBlockOutgoingBeam": true,
      "passwordBlockKeyguard": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordCountToBlock": 4,
      "passwordRequiredType": "required",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "safeBootBlocked": true,
      "screenCaptureBlocked": true,
      "securityAllowDebuggingFeatures": true,
      "securityRequireVerifyApps": true,
      "statusBarBlocked": true,
      "stayOnModes": [
        "ac"
      ],
      "storageAllowUsb": true,
      "storageBlockExternalMedia": true,
      "storageBlockUsbFileTransfer": true,
      "systemUpdateWindowStartMinutesAfterMidnight": 11,
      "systemUpdateWindowEndMinutesAfterMidnight": 9,
      "systemUpdateInstallType": "postpone",
      "usersBlockAdd": true,
      "usersBlockRemove": true,
      "volumeBlockAdjustment": true,
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true
    }
  ]
}
```





