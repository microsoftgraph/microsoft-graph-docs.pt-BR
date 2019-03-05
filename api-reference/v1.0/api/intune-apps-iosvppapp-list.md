---
title: Listar iosVppApps
description: Listar propriedades e relações dos objetos iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b159f9bdd02ce9299c0f459cd568e9118ea4a4f0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256424"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="712e2-103">Listar iosVppApps</span><span class="sxs-lookup"><span data-stu-id="712e2-103">List iosVppApps</span></span>

> <span data-ttu-id="712e2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="712e2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="712e2-105">Listar propriedades e relações dos objetos [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="712e2-105">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="712e2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="712e2-106">Prerequisites</span></span>
<span data-ttu-id="712e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="712e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="712e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="712e2-109">Permission type</span></span>|<span data-ttu-id="712e2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="712e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="712e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="712e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="712e2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="712e2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="712e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="712e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="712e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="712e2-114">Not supported.</span></span>|
|<span data-ttu-id="712e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="712e2-115">Application</span></span>|<span data-ttu-id="712e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="712e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="712e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="712e2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="712e2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="712e2-118">Request headers</span></span>
|<span data-ttu-id="712e2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="712e2-119">Header</span></span>|<span data-ttu-id="712e2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="712e2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="712e2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="712e2-121">Authorization</span></span>|<span data-ttu-id="712e2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="712e2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="712e2-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="712e2-123">Accept</span></span>|<span data-ttu-id="712e2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="712e2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="712e2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="712e2-125">Request body</span></span>
<span data-ttu-id="712e2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="712e2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="712e2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="712e2-127">Response</span></span>
<span data-ttu-id="712e2-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="712e2-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="712e2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="712e2-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="712e2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="712e2-130">Request</span></span>
<span data-ttu-id="712e2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="712e2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="712e2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="712e2-132">Response</span></span>
<span data-ttu-id="712e2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="712e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1575

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppApp",
      "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportsUserLicensing": true,
        "supportsDeviceLicensing": true
      },
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "vppTokenOrganizationName": "Vpp Token Organization Name value",
      "vppTokenAccountType": "education",
      "vppTokenAppleId": "Vpp Token Apple Id value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```



