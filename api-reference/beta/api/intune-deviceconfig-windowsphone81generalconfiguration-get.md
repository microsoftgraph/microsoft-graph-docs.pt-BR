---
title: Acessar windowsPhone81GeneralConfiguration
description: Leia as propriedades e as relações do objeto windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87bee64ee86bff2ec5e127455af47181e475eb54
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778492"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="4c813-103">Acessar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c813-103">Get windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="4c813-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c813-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c813-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c813-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c813-106">Leia as propriedades e as relações do objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c813-106">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c813-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c813-107">Prerequisites</span></span>
<span data-ttu-id="4c813-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c813-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c813-110">Permission type</span></span>|<span data-ttu-id="4c813-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c813-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c813-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c813-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c813-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c813-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4c813-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c813-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c813-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c813-115">Not supported.</span></span>|
|<span data-ttu-id="4c813-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c813-116">Application</span></span>|<span data-ttu-id="4c813-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c813-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c813-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c813-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c813-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c813-119">Optional query parameters</span></span>
<span data-ttu-id="4c813-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c813-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c813-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c813-121">Request headers</span></span>
|<span data-ttu-id="4c813-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c813-122">Header</span></span>|<span data-ttu-id="4c813-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4c813-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c813-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c813-124">Authorization</span></span>|<span data-ttu-id="4c813-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c813-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c813-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c813-126">Accept</span></span>|<span data-ttu-id="4c813-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4c813-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c813-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c813-128">Request body</span></span>
<span data-ttu-id="4c813-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c813-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c813-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c813-130">Response</span></span>
<span data-ttu-id="4c813-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c813-131">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c813-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c813-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c813-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c813-133">Request</span></span>
<span data-ttu-id="4c813-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c813-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4c813-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c813-135">Response</span></span>
<span data-ttu-id="4c813-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c813-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1840

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
    "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "applyOnlyToWindowsPhone81": true,
    "appsBlockCopyPaste": true,
    "bluetoothBlocked": true,
    "cameraBlocked": true,
    "cellularBlockWifiTethering": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "diagnosticDataBlockSubmission": true,
    "emailBlockAddingAccounts": true,
    "locationServicesBlocked": true,
    "microsoftAccountBlocked": true,
    "nfcBlocked": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "alphanumeric",
    "passwordRequired": true,
    "screenCaptureBlocked": true,
    "storageBlockRemovableStorage": true,
    "storageRequireEncryption": true,
    "webBrowserBlocked": true,
    "wifiBlocked": true,
    "wifiBlockAutomaticConnectHotspots": true,
    "wifiBlockHotspotReporting": true,
    "windowsStoreBlocked": true
  }
}
```





