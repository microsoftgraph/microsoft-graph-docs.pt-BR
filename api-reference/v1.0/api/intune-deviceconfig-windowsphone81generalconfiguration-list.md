---
title: Listar windowsPhone81GeneralConfigurations
description: Listar propriedades e relações dos objetos windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b28530a6b6b7a070c0a03a51a161242c84159722
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852931"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="2f8a5-103">Listar windowsPhone81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="2f8a5-103">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="2f8a5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2f8a5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f8a5-105">Listar propriedades e relações dos objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f8a5-105">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f8a5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f8a5-106">Prerequisites</span></span>
<span data-ttu-id="2f8a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f8a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f8a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f8a5-109">Permission type</span></span>|<span data-ttu-id="2f8a5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f8a5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f8a5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f8a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f8a5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f8a5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2f8a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f8a5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f8a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f8a5-114">Not supported.</span></span>|
|<span data-ttu-id="2f8a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f8a5-115">Application</span></span>|<span data-ttu-id="2f8a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f8a5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f8a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f8a5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f8a5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f8a5-118">Request headers</span></span>
|<span data-ttu-id="2f8a5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f8a5-119">Header</span></span>|<span data-ttu-id="2f8a5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2f8a5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f8a5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f8a5-121">Authorization</span></span>|<span data-ttu-id="2f8a5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f8a5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f8a5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f8a5-123">Accept</span></span>|<span data-ttu-id="2f8a5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f8a5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f8a5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f8a5-125">Request body</span></span>
<span data-ttu-id="2f8a5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f8a5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f8a5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f8a5-127">Response</span></span>
<span data-ttu-id="2f8a5-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f8a5-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f8a5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f8a5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f8a5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f8a5-130">Request</span></span>
<span data-ttu-id="2f8a5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f8a5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2f8a5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f8a5-132">Response</span></span>
<span data-ttu-id="2f8a5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f8a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1842

{
  "value": [
    {
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
  ]
}
```



