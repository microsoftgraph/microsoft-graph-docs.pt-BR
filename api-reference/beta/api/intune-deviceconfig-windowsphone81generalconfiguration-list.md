---
title: Listar windowsPhone81GeneralConfigurations
description: Listar propriedades e relações dos objetos windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 332ea956573e2f447a87e47779bdf176cd2a1987
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782195"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="fc33a-103">Listar windowsPhone81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="fc33a-103">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="fc33a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc33a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc33a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc33a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc33a-106">Listar propriedades e relações dos objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc33a-106">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc33a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc33a-107">Prerequisites</span></span>
<span data-ttu-id="fc33a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc33a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc33a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc33a-110">Permission type</span></span>|<span data-ttu-id="fc33a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc33a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc33a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc33a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc33a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc33a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fc33a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc33a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc33a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc33a-115">Not supported.</span></span>|
|<span data-ttu-id="fc33a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc33a-116">Application</span></span>|<span data-ttu-id="fc33a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc33a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc33a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc33a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fc33a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc33a-119">Request headers</span></span>
|<span data-ttu-id="fc33a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc33a-120">Header</span></span>|<span data-ttu-id="fc33a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fc33a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc33a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc33a-122">Authorization</span></span>|<span data-ttu-id="fc33a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc33a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc33a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc33a-124">Accept</span></span>|<span data-ttu-id="fc33a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc33a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc33a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc33a-126">Request body</span></span>
<span data-ttu-id="fc33a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc33a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc33a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc33a-128">Response</span></span>
<span data-ttu-id="fc33a-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc33a-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc33a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc33a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc33a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc33a-131">Request</span></span>
<span data-ttu-id="fc33a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc33a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fc33a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc33a-133">Response</span></span>
<span data-ttu-id="fc33a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc33a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1950

{
  "value": [
    {
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
  ]
}
```





