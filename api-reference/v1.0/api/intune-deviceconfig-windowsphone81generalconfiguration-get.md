---
title: Acessar windowsPhone81GeneralConfiguration
description: Leia as propriedades e as relações do objeto windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a063fd3f5e9d159abf2424963d4cf1435044e78d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967200"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="1db9d-103">Acessar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="1db9d-103">Get windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="1db9d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1db9d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1db9d-105">Leia as propriedades e as relações do objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1db9d-105">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1db9d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1db9d-106">Prerequisites</span></span>
<span data-ttu-id="1db9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1db9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1db9d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1db9d-109">Permission type</span></span>|<span data-ttu-id="1db9d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1db9d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1db9d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1db9d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1db9d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1db9d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1db9d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1db9d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1db9d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1db9d-114">Not supported.</span></span>|
|<span data-ttu-id="1db9d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1db9d-115">Application</span></span>|<span data-ttu-id="1db9d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1db9d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1db9d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1db9d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1db9d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1db9d-118">Optional query parameters</span></span>
<span data-ttu-id="1db9d-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1db9d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1db9d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1db9d-120">Request headers</span></span>
|<span data-ttu-id="1db9d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1db9d-121">Header</span></span>|<span data-ttu-id="1db9d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1db9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1db9d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1db9d-123">Authorization</span></span>|<span data-ttu-id="1db9d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1db9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1db9d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1db9d-125">Accept</span></span>|<span data-ttu-id="1db9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1db9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1db9d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1db9d-127">Request body</span></span>
<span data-ttu-id="1db9d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1db9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1db9d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1db9d-129">Response</span></span>
<span data-ttu-id="1db9d-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1db9d-130">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1db9d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1db9d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1db9d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1db9d-132">Request</span></span>
<span data-ttu-id="1db9d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1db9d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1db9d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1db9d-134">Response</span></span>
<span data-ttu-id="1db9d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1db9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1740

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
    "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



