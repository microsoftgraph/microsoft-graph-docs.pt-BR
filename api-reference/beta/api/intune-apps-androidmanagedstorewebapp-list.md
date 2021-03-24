---
title: Listar androidManagedStoreWebApps
description: Listar propriedades e relações dos objetos androidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f21b1e69b4a06c05e61ed2ffe0b472db6cf9c7b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140914"
---
# <a name="list-androidmanagedstorewebapps"></a><span data-ttu-id="0e8f8-103">Listar androidManagedStoreWebApps</span><span class="sxs-lookup"><span data-stu-id="0e8f8-103">List androidManagedStoreWebApps</span></span>

<span data-ttu-id="0e8f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e8f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e8f8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e8f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e8f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e8f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e8f8-107">Listar propriedades e relações dos objetos [androidManagedStoreWebApp.](../resources/intune-apps-androidmanagedstorewebapp.md)</span><span class="sxs-lookup"><span data-stu-id="0e8f8-107">List properties and relationships of the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e8f8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e8f8-108">Prerequisites</span></span>
<span data-ttu-id="0e8f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e8f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e8f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e8f8-111">Permission type</span></span>|<span data-ttu-id="0e8f8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e8f8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e8f8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e8f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e8f8-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e8f8-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e8f8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e8f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e8f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e8f8-116">Not supported.</span></span>|
|<span data-ttu-id="0e8f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e8f8-117">Application</span></span>|<span data-ttu-id="0e8f8-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e8f8-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e8f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e8f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0e8f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e8f8-120">Request headers</span></span>
|<span data-ttu-id="0e8f8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e8f8-121">Header</span></span>|<span data-ttu-id="0e8f8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e8f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e8f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e8f8-123">Authorization</span></span>|<span data-ttu-id="0e8f8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e8f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e8f8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e8f8-125">Accept</span></span>|<span data-ttu-id="0e8f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e8f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e8f8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e8f8-127">Request body</span></span>
<span data-ttu-id="0e8f8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e8f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e8f8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e8f8-129">Response</span></span>
<span data-ttu-id="0e8f8-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e8f8-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e8f8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e8f8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e8f8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e8f8-132">Request</span></span>
<span data-ttu-id="0e8f8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e8f8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="0e8f8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e8f8-134">Response</span></span>
<span data-ttu-id="0e8f8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e8f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1601

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
      "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "isPrivate": true,
      "isSystemApp": true,
      "appTracks": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
          "trackId": "Track Id value",
          "trackAlias": "Track Alias value"
        }
      ],
      "supportsOemConfig": true
    }
  ]
}
```




