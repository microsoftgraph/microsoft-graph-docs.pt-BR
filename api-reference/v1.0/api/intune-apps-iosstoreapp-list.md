---
title: Listar iosStoreApps
description: Listar propriedades e relações dos objetos iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd0708d77cbf3514f5778c1881b690fcc7acbeeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997873"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="20b48-103">Listar iosStoreApps</span><span class="sxs-lookup"><span data-stu-id="20b48-103">List iosStoreApps</span></span>

> <span data-ttu-id="20b48-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20b48-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20b48-105">Listar propriedades e relações dos objetos [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="20b48-105">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20b48-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20b48-106">Prerequisites</span></span>
<span data-ttu-id="20b48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20b48-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20b48-109">Permission type</span></span>|<span data-ttu-id="20b48-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20b48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20b48-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20b48-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20b48-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b48-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="20b48-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20b48-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20b48-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20b48-114">Not supported.</span></span>|
|<span data-ttu-id="20b48-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20b48-115">Application</span></span>|<span data-ttu-id="20b48-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20b48-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20b48-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20b48-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="20b48-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20b48-118">Request headers</span></span>
|<span data-ttu-id="20b48-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20b48-119">Header</span></span>|<span data-ttu-id="20b48-120">Valor</span><span class="sxs-lookup"><span data-stu-id="20b48-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20b48-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="20b48-121">Authorization</span></span>|<span data-ttu-id="20b48-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20b48-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20b48-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="20b48-123">Accept</span></span>|<span data-ttu-id="20b48-124">application/json</span><span class="sxs-lookup"><span data-stu-id="20b48-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b48-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20b48-125">Request body</span></span>
<span data-ttu-id="20b48-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20b48-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20b48-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="20b48-127">Response</span></span>
<span data-ttu-id="20b48-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20b48-128">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20b48-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20b48-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="20b48-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20b48-130">Request</span></span>
<span data-ttu-id="20b48-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20b48-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="20b48-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="20b48-132">Response</span></span>
<span data-ttu-id="20b48-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20b48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1347

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
        "v12_0": true
      }
    }
  ]
}
```



