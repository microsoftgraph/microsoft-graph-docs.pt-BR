---
title: Listar iosStoreApps
description: Listar propriedades e relações dos objetos iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c25a1a46864dc1e605a9c7f7624d8b3f9fd70be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070132"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="f8cb7-103">Listar iosStoreApps</span><span class="sxs-lookup"><span data-stu-id="f8cb7-103">List iosStoreApps</span></span>

<span data-ttu-id="f8cb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8cb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8cb7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8cb7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8cb7-106">Listar propriedades e relações dos objetos [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f8cb7-106">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8cb7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8cb7-107">Prerequisites</span></span>
<span data-ttu-id="f8cb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8cb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f8cb7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8cb7-110">Permission type</span></span>|<span data-ttu-id="f8cb7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8cb7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8cb7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8cb7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8cb7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8cb7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f8cb7-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8cb7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8cb7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8cb7-115">Not supported.</span></span>|
|<span data-ttu-id="f8cb7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8cb7-116">Application</span></span>|<span data-ttu-id="f8cb7-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8cb7-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8cb7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8cb7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f8cb7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8cb7-119">Request headers</span></span>
|<span data-ttu-id="f8cb7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8cb7-120">Header</span></span>|<span data-ttu-id="f8cb7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8cb7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8cb7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8cb7-122">Authorization</span></span>|<span data-ttu-id="f8cb7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8cb7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8cb7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8cb7-124">Accept</span></span>|<span data-ttu-id="f8cb7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8cb7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8cb7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8cb7-126">Request body</span></span>
<span data-ttu-id="f8cb7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8cb7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8cb7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8cb7-128">Response</span></span>
<span data-ttu-id="f8cb7-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8cb7-129">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8cb7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8cb7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8cb7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8cb7-131">Request</span></span>
<span data-ttu-id="f8cb7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8cb7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f8cb7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8cb7-133">Response</span></span>
<span data-ttu-id="f8cb7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8cb7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1371

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosStoreApp",
      "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
        "v12_0": true,
        "v13_0": true
      }
    }
  ]
}
```









