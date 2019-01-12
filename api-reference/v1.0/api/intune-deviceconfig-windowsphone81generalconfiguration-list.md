---
title: Listar windowsPhone81GeneralConfigurations
description: Listar propriedades e relações dos objetos windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb4e4acad6074093778b53bf9dff1484e549b1ed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947257"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="55174-103">Listar windowsPhone81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="55174-103">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="55174-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="55174-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55174-105">Listar propriedades e relações dos objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55174-105">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55174-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55174-106">Prerequisites</span></span>
<span data-ttu-id="55174-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55174-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55174-109">Permission type</span></span>|<span data-ttu-id="55174-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55174-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55174-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55174-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55174-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="55174-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="55174-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55174-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55174-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55174-114">Not supported.</span></span>|
|<span data-ttu-id="55174-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55174-115">Application</span></span>|<span data-ttu-id="55174-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55174-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55174-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55174-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="55174-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55174-118">Request headers</span></span>
|<span data-ttu-id="55174-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55174-119">Header</span></span>|<span data-ttu-id="55174-120">Valor</span><span class="sxs-lookup"><span data-stu-id="55174-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55174-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55174-121">Authorization</span></span>|<span data-ttu-id="55174-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55174-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55174-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55174-123">Accept</span></span>|<span data-ttu-id="55174-124">application/json</span><span class="sxs-lookup"><span data-stu-id="55174-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55174-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55174-125">Request body</span></span>
<span data-ttu-id="55174-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55174-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55174-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="55174-127">Response</span></span>
<span data-ttu-id="55174-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55174-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55174-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55174-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="55174-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55174-130">Request</span></span>
<span data-ttu-id="55174-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55174-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="55174-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="55174-132">Response</span></span>
<span data-ttu-id="55174-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55174-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



