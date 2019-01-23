---
title: Lista win32LobApps
description: Lista as propriedades e os relacionamentos dos objetos win32LobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c8e9678b0c4833fd3aaccec36e78bade1d03b7c3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417606"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="f5501-103">Lista win32LobApps</span><span class="sxs-lookup"><span data-stu-id="f5501-103">List win32LobApps</span></span>

> <span data-ttu-id="f5501-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5501-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5501-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5501-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5501-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f5501-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5501-107">Lista as propriedades e os relacionamentos dos objetos [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f5501-107">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5501-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5501-108">Prerequisites</span></span>
<span data-ttu-id="f5501-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5501-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f5501-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5501-111">Permission type</span></span>|<span data-ttu-id="f5501-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5501-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5501-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5501-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5501-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5501-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f5501-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5501-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5501-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5501-116">Not supported.</span></span>|
|<span data-ttu-id="f5501-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5501-117">Application</span></span>|<span data-ttu-id="f5501-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5501-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5501-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5501-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f5501-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5501-120">Request headers</span></span>
|<span data-ttu-id="f5501-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5501-121">Header</span></span>|<span data-ttu-id="f5501-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5501-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5501-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5501-123">Authorization</span></span>|<span data-ttu-id="f5501-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5501-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5501-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5501-125">Accept</span></span>|<span data-ttu-id="f5501-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5501-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5501-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5501-127">Request body</span></span>
<span data-ttu-id="f5501-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5501-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5501-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5501-129">Response</span></span>
<span data-ttu-id="f5501-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5501-130">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5501-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5501-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5501-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5501-132">Request</span></span>
<span data-ttu-id="f5501-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5501-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f5501-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5501-134">Response</span></span>
<span data-ttu-id="f5501-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5501-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2790

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.win32LobApp",
      "id": "9607b530-b530-9607-30b5-079630b50796",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "installCommandLine": "Install Command Line value",
      "uninstallCommandLine": "Uninstall Command Line value",
      "applicableArchitectures": "x86",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      },
      "minimumFreeDiskSpaceInMB": 8,
      "minimumMemoryInMB": 1,
      "minimumNumberOfProcessors": 9,
      "minimumCpuSpeedInMHz": 4,
      "detectionRules": [
        {
          "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
          "check32BitOn64System": true,
          "keyPath": "Key Path value",
          "valueName": "Value Name value",
          "detectionType": "exists",
          "operator": "equal",
          "detectionValue": "Detection Value value"
        }
      ],
      "installExperience": {
        "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
        "runAsAccount": "user"
      },
      "returnCodes": [
        {
          "@odata.type": "microsoft.graph.win32LobAppReturnCode",
          "returnCode": 10,
          "type": "success"
        }
      ],
      "msiInformation": {
        "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
        "productCode": "Product Code value",
        "productVersion": "Product Version value",
        "upgradeCode": "Upgrade Code value",
        "requiresReboot": true,
        "packageType": "perUser"
      },
      "setupFilePath": "Setup File Path value"
    }
  ]
}
```




