---
title: Acessar windowsPhone81GeneralConfiguration
description: Leia as propriedades e as relações do objeto windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b5355a6015c6686983cd168f982de1316f4db50
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757014"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="7c210-103">Acessar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c210-103">Get windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="7c210-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c210-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c210-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c210-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c210-106">Leia as propriedades e as relações do objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c210-106">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c210-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c210-107">Prerequisites</span></span>
<span data-ttu-id="7c210-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c210-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c210-110">Permission type</span></span>|<span data-ttu-id="7c210-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c210-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c210-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c210-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c210-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c210-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c210-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c210-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c210-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c210-115">Not supported.</span></span>|
|<span data-ttu-id="7c210-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c210-116">Application</span></span>|<span data-ttu-id="7c210-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c210-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c210-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c210-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c210-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c210-119">Optional query parameters</span></span>
<span data-ttu-id="7c210-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c210-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c210-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c210-121">Request headers</span></span>
|<span data-ttu-id="7c210-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c210-122">Header</span></span>|<span data-ttu-id="7c210-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7c210-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c210-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c210-124">Authorization</span></span>|<span data-ttu-id="7c210-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c210-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c210-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c210-126">Accept</span></span>|<span data-ttu-id="7c210-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c210-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c210-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c210-128">Request body</span></span>
<span data-ttu-id="7c210-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c210-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c210-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c210-130">Response</span></span>
<span data-ttu-id="7c210-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c210-131">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c210-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c210-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c210-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c210-133">Request</span></span>
<span data-ttu-id="7c210-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c210-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7c210-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c210-135">Response</span></span>
<span data-ttu-id="7c210-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c210-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




