---
title: Listar managedIOSStoreApps
description: Listar propriedades e relações dos objetos managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52cd1fcf46dc25916f507e4c67f7d13b587c6fde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453940"
---
# <a name="list-managediosstoreapps"></a><span data-ttu-id="5a886-103">Listar managedIOSStoreApps</span><span class="sxs-lookup"><span data-stu-id="5a886-103">List managedIOSStoreApps</span></span>

> <span data-ttu-id="5a886-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a886-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a886-105">Listar propriedades e relações dos objetos [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a886-105">List properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a886-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a886-106">Prerequisites</span></span>
<span data-ttu-id="5a886-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a886-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a886-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a886-109">Permission type</span></span>|<span data-ttu-id="5a886-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a886-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a886-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a886-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a886-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a886-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5a886-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a886-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a886-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a886-114">Not supported.</span></span>|
|<span data-ttu-id="5a886-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a886-115">Application</span></span>|<span data-ttu-id="5a886-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a886-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a886-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a886-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5a886-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a886-118">Request headers</span></span>
|<span data-ttu-id="5a886-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a886-119">Header</span></span>|<span data-ttu-id="5a886-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5a886-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a886-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a886-121">Authorization</span></span>|<span data-ttu-id="5a886-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a886-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a886-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a886-123">Accept</span></span>|<span data-ttu-id="5a886-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a886-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a886-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a886-125">Request body</span></span>
<span data-ttu-id="5a886-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a886-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a886-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a886-127">Response</span></span>
<span data-ttu-id="5a886-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a886-128">If successful, this method returns a `200 OK` response code and a collection of [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a886-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a886-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a886-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a886-130">Request</span></span>
<span data-ttu-id="5a886-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a886-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="5a886-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a886-132">Response</span></span>
<span data-ttu-id="5a886-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a886-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1433

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
      "publishingState": "processing",
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



