---
title: Listar managedIOSStoreApps
description: Listar propriedades e relações dos objetos managedIOSStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8334e09bae193da942e7831086a3c3f89d69adf3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935486"
---
# <a name="list-managediosstoreapps"></a><span data-ttu-id="f9dd9-103">Listar managedIOSStoreApps</span><span class="sxs-lookup"><span data-stu-id="f9dd9-103">List managedIOSStoreApps</span></span>

> <span data-ttu-id="f9dd9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9dd9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9dd9-106">Listar propriedades e relações dos objetos [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9dd9-106">List properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9dd9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9dd9-107">Prerequisites</span></span>
<span data-ttu-id="f9dd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9dd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9dd9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9dd9-110">Permission type</span></span>|<span data-ttu-id="f9dd9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9dd9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9dd9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9dd9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9dd9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9dd9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f9dd9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9dd9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9dd9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-115">Not supported.</span></span>|
|<span data-ttu-id="f9dd9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9dd9-116">Application</span></span>|<span data-ttu-id="f9dd9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9dd9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9dd9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f9dd9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9dd9-119">Request headers</span></span>
|<span data-ttu-id="f9dd9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9dd9-120">Header</span></span>|<span data-ttu-id="f9dd9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f9dd9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9dd9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9dd9-122">Authorization</span></span>|<span data-ttu-id="f9dd9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9dd9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9dd9-124">Accept</span></span>|<span data-ttu-id="f9dd9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9dd9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9dd9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9dd9-126">Request body</span></span>
<span data-ttu-id="f9dd9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9dd9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9dd9-128">Response</span></span>
<span data-ttu-id="f9dd9-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-129">If successful, this method returns a `200 OK` response code and a collection of [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9dd9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9dd9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9dd9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9dd9-131">Request</span></span>
<span data-ttu-id="f9dd9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f9dd9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9dd9-133">Response</span></span>
<span data-ttu-id="f9dd9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9dd9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1591

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSStoreApp",
      "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "bundleId": "Bundle Id value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
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
        "v12_0": true
      }
    }
  ]
}
```




