---
title: Listar managedIOSLobApps
description: Listar propriedades e relações dos objetos managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19bc261470ea01731e5a021c9da1fb7455253c25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977786"
---
# <a name="list-managedioslobapps"></a><span data-ttu-id="54968-103">Listar managedIOSLobApps</span><span class="sxs-lookup"><span data-stu-id="54968-103">List managedIOSLobApps</span></span>

<span data-ttu-id="54968-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54968-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54968-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54968-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54968-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54968-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54968-107">Listar propriedades e relações dos objetos [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="54968-107">List properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54968-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54968-108">Prerequisites</span></span>
<span data-ttu-id="54968-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54968-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54968-111">Permission type</span></span>|<span data-ttu-id="54968-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54968-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54968-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54968-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54968-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="54968-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="54968-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54968-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54968-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54968-116">Not supported.</span></span>|
|<span data-ttu-id="54968-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54968-117">Application</span></span>|<span data-ttu-id="54968-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="54968-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54968-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54968-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="54968-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54968-120">Request headers</span></span>
|<span data-ttu-id="54968-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54968-121">Header</span></span>|<span data-ttu-id="54968-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54968-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54968-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54968-123">Authorization</span></span>|<span data-ttu-id="54968-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54968-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54968-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54968-125">Accept</span></span>|<span data-ttu-id="54968-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54968-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54968-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54968-127">Request body</span></span>
<span data-ttu-id="54968-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54968-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54968-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="54968-129">Response</span></span>
<span data-ttu-id="54968-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54968-130">If successful, this method returns a `200 OK` response code and a collection of [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54968-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54968-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="54968-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54968-132">Request</span></span>
<span data-ttu-id="54968-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54968-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="54968-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="54968-134">Response</span></span>
<span data-ttu-id="54968-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54968-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1955

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSLobApp",
      "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
      "dependentAppCount": 1,
      "supersedingAppCount": 3,
      "supersededAppCount": 2,
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "bundleId": "Bundle Id value",
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
        "v8_0": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true,
        "v12_0": true,
        "v13_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```






