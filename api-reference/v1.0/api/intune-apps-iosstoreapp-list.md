---
title: Listar iosStoreApps
description: Listar propriedades e relações dos objetos iosStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bc0355f79412137880022465b94ddd50d814142
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516529"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="d21dd-103">Listar iosStoreApps</span><span class="sxs-lookup"><span data-stu-id="d21dd-103">List iosStoreApps</span></span>

<span data-ttu-id="d21dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d21dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d21dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d21dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d21dd-106">Listar propriedades e relações dos objetos [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="d21dd-106">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d21dd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d21dd-107">Prerequisites</span></span>
<span data-ttu-id="d21dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d21dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d21dd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d21dd-110">Permission type</span></span>|<span data-ttu-id="d21dd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d21dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d21dd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d21dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d21dd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d21dd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d21dd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d21dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d21dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d21dd-115">Not supported.</span></span>|
|<span data-ttu-id="d21dd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d21dd-116">Application</span></span>|<span data-ttu-id="d21dd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d21dd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d21dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d21dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d21dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d21dd-119">Request headers</span></span>
|<span data-ttu-id="d21dd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d21dd-120">Header</span></span>|<span data-ttu-id="d21dd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d21dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d21dd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d21dd-122">Authorization</span></span>|<span data-ttu-id="d21dd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d21dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d21dd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d21dd-124">Accept</span></span>|<span data-ttu-id="d21dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d21dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d21dd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d21dd-126">Request body</span></span>
<span data-ttu-id="d21dd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d21dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d21dd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d21dd-128">Response</span></span>
<span data-ttu-id="d21dd-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d21dd-129">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d21dd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d21dd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d21dd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d21dd-131">Request</span></span>
<span data-ttu-id="d21dd-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d21dd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="d21dd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d21dd-133">Response</span></span>
<span data-ttu-id="d21dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d21dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




