---
title: Listar microsoftStoreForBusinessApps
description: Listar propriedades e relações dos objetos microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe78ffd739f2b8cb926843333f8867b9dbb33944
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961200"
---
# <a name="list-microsoftstoreforbusinessapps"></a><span data-ttu-id="363f4-103">Listar microsoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="363f4-103">List microsoftStoreForBusinessApps</span></span>

> <span data-ttu-id="363f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="363f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="363f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="363f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="363f4-106">Listar propriedades e relações dos objetos [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="363f4-106">List properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="363f4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="363f4-107">Prerequisites</span></span>
<span data-ttu-id="363f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="363f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="363f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="363f4-110">Permission type</span></span>|<span data-ttu-id="363f4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="363f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="363f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="363f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="363f4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="363f4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="363f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="363f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="363f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="363f4-115">Not supported.</span></span>|
|<span data-ttu-id="363f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="363f4-116">Application</span></span>|<span data-ttu-id="363f4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="363f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="363f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="363f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="363f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="363f4-119">Request headers</span></span>
|<span data-ttu-id="363f4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="363f4-120">Header</span></span>|<span data-ttu-id="363f4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="363f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="363f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="363f4-122">Authorization</span></span>|<span data-ttu-id="363f4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="363f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="363f4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="363f4-124">Accept</span></span>|<span data-ttu-id="363f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="363f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="363f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="363f4-126">Request body</span></span>
<span data-ttu-id="363f4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="363f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="363f4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="363f4-128">Response</span></span>
<span data-ttu-id="363f4-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="363f4-129">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="363f4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="363f4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="363f4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="363f4-131">Request</span></span>
<span data-ttu-id="363f4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="363f4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="363f4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="363f4-133">Response</span></span>
<span data-ttu-id="363f4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="363f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1485

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
      "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "productKey": "Product Key value",
      "licenseType": "online",
      "packageIdentityName": "Package Identity Name value",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportUserLicensing": true,
        "supportDeviceLicensing": true,
        "supportsUserLicensing": true,
        "supportsDeviceLicensing": true
      }
    }
  ]
}
```





