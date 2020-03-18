---
title: Listar androidManagedStoreApps
description: Listar Propriedades e relações dos objetos androidManagedStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 609f4c98e2acd39f04d89f9a1e5a19ad99014f1e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762277"
---
# <a name="list-androidmanagedstoreapps"></a><span data-ttu-id="c07e9-103">Listar androidManagedStoreApps</span><span class="sxs-lookup"><span data-stu-id="c07e9-103">List androidManagedStoreApps</span></span>

> <span data-ttu-id="c07e9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c07e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c07e9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c07e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c07e9-106">Listar Propriedades e relações dos objetos [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c07e9-106">List properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c07e9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c07e9-107">Prerequisites</span></span>
<span data-ttu-id="c07e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c07e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c07e9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c07e9-110">Permission type</span></span>|<span data-ttu-id="c07e9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c07e9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c07e9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c07e9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c07e9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c07e9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c07e9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c07e9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c07e9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c07e9-115">Not supported.</span></span>|
|<span data-ttu-id="c07e9-116">Application</span><span class="sxs-lookup"><span data-stu-id="c07e9-116">Application</span></span>|<span data-ttu-id="c07e9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c07e9-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c07e9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c07e9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c07e9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c07e9-119">Request headers</span></span>
|<span data-ttu-id="c07e9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c07e9-120">Header</span></span>|<span data-ttu-id="c07e9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c07e9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c07e9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c07e9-122">Authorization</span></span>|<span data-ttu-id="c07e9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c07e9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c07e9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c07e9-124">Accept</span></span>|<span data-ttu-id="c07e9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c07e9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c07e9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c07e9-126">Request body</span></span>
<span data-ttu-id="c07e9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c07e9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c07e9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c07e9-128">Response</span></span>
<span data-ttu-id="c07e9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c07e9-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c07e9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c07e9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c07e9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c07e9-131">Request</span></span>
<span data-ttu-id="c07e9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c07e9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="c07e9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c07e9-133">Response</span></span>
<span data-ttu-id="c07e9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c07e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1321

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreApp",
      "id": "87247525-7525-8724-2575-248725752487",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "isPrivate": true,
      "isSystemApp": true,
      "supportsOemConfig": true
    }
  ]
}
```




