---
title: Listar windowsPhone81GeneralConfigurations
description: Listar propriedades e relações dos objetos windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d462cfa2a1d29ce3a0cc2cedf54cc0113e3147a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009643"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="46b09-103">Listar windowsPhone81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="46b09-103">List windowsPhone81GeneralConfigurations</span></span>

<span data-ttu-id="46b09-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46b09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46b09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46b09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46b09-106">Listar propriedades e relações dos objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46b09-106">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46b09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46b09-107">Prerequisites</span></span>
<span data-ttu-id="46b09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46b09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46b09-110">Permission type</span></span>|<span data-ttu-id="46b09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46b09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46b09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46b09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46b09-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="46b09-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="46b09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46b09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46b09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46b09-115">Not supported.</span></span>|
|<span data-ttu-id="46b09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46b09-116">Application</span></span>|<span data-ttu-id="46b09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46b09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46b09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46b09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="46b09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46b09-119">Request headers</span></span>
|<span data-ttu-id="46b09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46b09-120">Header</span></span>|<span data-ttu-id="46b09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46b09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46b09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46b09-122">Authorization</span></span>|<span data-ttu-id="46b09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46b09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46b09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46b09-124">Accept</span></span>|<span data-ttu-id="46b09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46b09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46b09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46b09-126">Request body</span></span>
<span data-ttu-id="46b09-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46b09-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46b09-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b09-128">Response</span></span>
<span data-ttu-id="46b09-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46b09-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b09-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46b09-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46b09-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46b09-131">Request</span></span>
<span data-ttu-id="46b09-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46b09-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="46b09-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46b09-133">Response</span></span>
<span data-ttu-id="46b09-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46b09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









