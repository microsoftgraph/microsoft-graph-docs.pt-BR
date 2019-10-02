---
title: Listar iosLobApps
description: Listar propriedades e relações dos objetos iosLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33f0d6c1d4968dda3c8cb561cbbcf80a90cec823
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358912"
---
# <a name="list-ioslobapps"></a><span data-ttu-id="a31d5-103">Listar iosLobApps</span><span class="sxs-lookup"><span data-stu-id="a31d5-103">List iosLobApps</span></span>

> <span data-ttu-id="a31d5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a31d5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a31d5-105">Listar propriedades e relações dos objetos [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a31d5-105">List properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a31d5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a31d5-106">Prerequisites</span></span>
<span data-ttu-id="a31d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a31d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a31d5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a31d5-109">Permission type</span></span>|<span data-ttu-id="a31d5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a31d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a31d5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a31d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a31d5-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a31d5-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a31d5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a31d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a31d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a31d5-114">Not supported.</span></span>|
|<span data-ttu-id="a31d5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a31d5-115">Application</span></span>|<span data-ttu-id="a31d5-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a31d5-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a31d5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a31d5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a31d5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a31d5-118">Request headers</span></span>
|<span data-ttu-id="a31d5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a31d5-119">Header</span></span>|<span data-ttu-id="a31d5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a31d5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a31d5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a31d5-121">Authorization</span></span>|<span data-ttu-id="a31d5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a31d5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a31d5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a31d5-123">Accept</span></span>|<span data-ttu-id="a31d5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a31d5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a31d5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a31d5-125">Request body</span></span>
<span data-ttu-id="a31d5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a31d5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a31d5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a31d5-127">Response</span></span>
<span data-ttu-id="a31d5-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a31d5-128">If successful, this method returns a `200 OK` response code and a collection of [iosLobApp](../resources/intune-apps-ioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a31d5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a31d5-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a31d5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a31d5-130">Request</span></span>
<span data-ttu-id="a31d5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a31d5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a31d5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a31d5-132">Response</span></span>
<span data-ttu-id="a31d5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a31d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1594

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobApp",
      "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
      "buildNumber": "Build Number value"
    }
  ]
}
```




