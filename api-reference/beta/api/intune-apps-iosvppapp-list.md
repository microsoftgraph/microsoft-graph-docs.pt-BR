---
title: Listar iosVppApps
description: Listar propriedades e relações dos objetos iosVppApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 14b670daffdc7266397c8c090ec3ae49ea66c46b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418005"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="a6322-103">Listar iosVppApps</span><span class="sxs-lookup"><span data-stu-id="a6322-103">List iosVppApps</span></span>

> <span data-ttu-id="a6322-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6322-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6322-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6322-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6322-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a6322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6322-107">Listar propriedades e relações dos objetos [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6322-107">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6322-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6322-108">Prerequisites</span></span>
<span data-ttu-id="a6322-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6322-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6322-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6322-111">Permission type</span></span>|<span data-ttu-id="a6322-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6322-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6322-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6322-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6322-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6322-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a6322-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6322-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6322-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6322-116">Not supported.</span></span>|
|<span data-ttu-id="a6322-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6322-117">Application</span></span>|<span data-ttu-id="a6322-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6322-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6322-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6322-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a6322-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6322-120">Request headers</span></span>
|<span data-ttu-id="a6322-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6322-121">Header</span></span>|<span data-ttu-id="a6322-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6322-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6322-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6322-123">Authorization</span></span>|<span data-ttu-id="a6322-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6322-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6322-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6322-125">Accept</span></span>|<span data-ttu-id="a6322-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6322-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6322-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6322-127">Request body</span></span>
<span data-ttu-id="a6322-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6322-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6322-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6322-129">Response</span></span>
<span data-ttu-id="a6322-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6322-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6322-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6322-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6322-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6322-132">Request</span></span>
<span data-ttu-id="a6322-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6322-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a6322-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6322-134">Response</span></span>
<span data-ttu-id="a6322-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6322-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2413

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
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportUserLicensing": true,
        "supportDeviceLicensing": true,
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
      "bundleId": "Bundle Id value",
      "vppTokenId": "Vpp Token Id value",
      "revokeLicenseActionResults": [
        {
          "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
          "userId": "User Id value",
          "managedDeviceId": "Managed Device Id value",
          "totalLicensesCount": 2,
          "failedLicensesCount": 3,
          "actionFailureReason": "appleFailure",
          "actionName": "Action Name value",
          "actionState": "pending",
          "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
          "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
        }
      ]
    }
  ]
}
```




