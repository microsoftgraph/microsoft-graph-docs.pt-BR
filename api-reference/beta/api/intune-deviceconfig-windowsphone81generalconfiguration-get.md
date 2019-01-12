---
title: Acessar windowsPhone81GeneralConfiguration
description: Leia as propriedades e as relações do objeto windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a623fbf19d2d779ecfb7dce755a320544f28f0fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944709"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="67135-103">Acessar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="67135-103">Get windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="67135-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="67135-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67135-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67135-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67135-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="67135-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67135-107">Leia as propriedades e as relações do objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67135-107">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67135-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67135-108">Prerequisites</span></span>
<span data-ttu-id="67135-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67135-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67135-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67135-111">Permission type</span></span>|<span data-ttu-id="67135-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67135-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67135-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67135-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67135-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="67135-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="67135-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67135-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67135-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67135-116">Not supported.</span></span>|
|<span data-ttu-id="67135-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67135-117">Application</span></span>|<span data-ttu-id="67135-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67135-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67135-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67135-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67135-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="67135-120">Optional query parameters</span></span>
<span data-ttu-id="67135-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="67135-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="67135-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67135-122">Request headers</span></span>
|<span data-ttu-id="67135-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67135-123">Header</span></span>|<span data-ttu-id="67135-124">Valor</span><span class="sxs-lookup"><span data-stu-id="67135-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67135-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="67135-125">Authorization</span></span>|<span data-ttu-id="67135-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67135-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67135-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67135-127">Accept</span></span>|<span data-ttu-id="67135-128">application/json</span><span class="sxs-lookup"><span data-stu-id="67135-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67135-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67135-129">Request body</span></span>
<span data-ttu-id="67135-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67135-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67135-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="67135-131">Response</span></span>
<span data-ttu-id="67135-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67135-132">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67135-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67135-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="67135-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67135-134">Request</span></span>
<span data-ttu-id="67135-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67135-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="67135-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="67135-136">Response</span></span>
<span data-ttu-id="67135-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67135-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





