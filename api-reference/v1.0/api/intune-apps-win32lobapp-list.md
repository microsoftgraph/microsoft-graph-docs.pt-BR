---
title: Listar win32LobApps
description: Listar propriedades e relações dos objetos win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec407801c60990bb93c802aa4682e28566d62c8b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758726"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="2d166-103">Listar win32LobApps</span><span class="sxs-lookup"><span data-stu-id="2d166-103">List win32LobApps</span></span>

<span data-ttu-id="2d166-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d166-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d166-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d166-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d166-106">Listar propriedades e relações dos [objetos win32LobApp.](../resources/intune-apps-win32lobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d166-106">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d166-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d166-107">Prerequisites</span></span>
<span data-ttu-id="2d166-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d166-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d166-110">Permission type</span></span>|<span data-ttu-id="2d166-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d166-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d166-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d166-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d166-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d166-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d166-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d166-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d166-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d166-115">Not supported.</span></span>|
|<span data-ttu-id="2d166-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d166-116">Application</span></span>|<span data-ttu-id="2d166-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d166-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d166-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d166-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2d166-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d166-119">Request headers</span></span>
|<span data-ttu-id="2d166-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d166-120">Header</span></span>|<span data-ttu-id="2d166-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2d166-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d166-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d166-122">Authorization</span></span>|<span data-ttu-id="2d166-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d166-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d166-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d166-124">Accept</span></span>|<span data-ttu-id="2d166-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d166-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d166-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d166-126">Request body</span></span>
<span data-ttu-id="2d166-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d166-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d166-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d166-128">Response</span></span>
<span data-ttu-id="2d166-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d166-129">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d166-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d166-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d166-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d166-131">Request</span></span>
<span data-ttu-id="2d166-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d166-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2d166-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d166-133">Response</span></span>
<span data-ttu-id="2d166-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d166-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2599

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
      "publishingState": "processing",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "installCommandLine": "Install Command Line value",
      "uninstallCommandLine": "Uninstall Command Line value",
      "applicableArchitectures": "x86",
      "minimumFreeDiskSpaceInMB": 8,
      "minimumMemoryInMB": 1,
      "minimumNumberOfProcessors": 9,
      "minimumCpuSpeedInMHz": 4,
      "rules": [
        {
          "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
          "ruleType": "requirement",
          "check32BitOn64System": true,
          "keyPath": "Key Path value",
          "valueName": "Value Name value",
          "operationType": "exists",
          "operator": "equal",
          "comparisonValue": "Comparison Value value"
        }
      ],
      "installExperience": {
        "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
        "runAsAccount": "user",
        "deviceRestartBehavior": "allow"
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
        "packageType": "perUser",
        "productName": "Product Name value",
        "publisher": "Publisher value"
      },
      "setupFilePath": "Setup File Path value",
      "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
    }
  ]
}
```




