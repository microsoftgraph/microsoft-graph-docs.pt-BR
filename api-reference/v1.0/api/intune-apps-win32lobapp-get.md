---
title: Obter win32LobApp
description: Leia as propriedades e as relações do objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4dc7275cccae7986e2ea1a379b24aef264c34097
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080025"
---
# <a name="get-win32lobapp"></a><span data-ttu-id="bf782-103">Obter win32LobApp</span><span class="sxs-lookup"><span data-stu-id="bf782-103">Get win32LobApp</span></span>

<span data-ttu-id="bf782-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf782-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf782-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf782-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf782-106">Leia as propriedades e as relações do objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bf782-106">Read properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf782-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bf782-107">Prerequisites</span></span>
<span data-ttu-id="bf782-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf782-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf782-110">Permission type</span></span>|<span data-ttu-id="bf782-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bf782-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf782-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf782-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf782-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf782-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bf782-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf782-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf782-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf782-115">Not supported.</span></span>|
|<span data-ttu-id="bf782-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf782-116">Application</span></span>|<span data-ttu-id="bf782-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf782-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf782-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf782-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf782-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bf782-119">Optional query parameters</span></span>
<span data-ttu-id="bf782-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bf782-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf782-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf782-121">Request headers</span></span>
|<span data-ttu-id="bf782-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf782-122">Header</span></span>|<span data-ttu-id="bf782-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bf782-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf782-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf782-124">Authorization</span></span>|<span data-ttu-id="bf782-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf782-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf782-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bf782-126">Accept</span></span>|<span data-ttu-id="bf782-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bf782-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf782-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf782-128">Request body</span></span>
<span data-ttu-id="bf782-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf782-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf782-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf782-130">Response</span></span>
<span data-ttu-id="bf782-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf782-131">If successful, this method returns a `200 OK` response code and [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf782-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf782-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf782-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf782-133">Request</span></span>
<span data-ttu-id="bf782-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf782-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="bf782-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf782-135">Response</span></span>
<span data-ttu-id="bf782-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf782-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2455

{
  "value": {
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
}
```






