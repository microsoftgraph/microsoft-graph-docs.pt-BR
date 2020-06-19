---
title: Listar officeSuiteApps
description: Listar Propriedades e relações dos objetos officeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27502115c5e67bf5bf432161d95e4a22f9957b16
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793280"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="fe684-103">Listar officeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="fe684-103">List officeSuiteApps</span></span>

<span data-ttu-id="fe684-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe684-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe684-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe684-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe684-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe684-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe684-107">Listar Propriedades e relações dos objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fe684-107">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe684-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe684-108">Prerequisites</span></span>
<span data-ttu-id="fe684-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fe684-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fe684-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe684-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe684-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe684-111">Permission type</span></span>|<span data-ttu-id="fe684-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe684-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe684-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe684-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe684-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe684-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fe684-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe684-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe684-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe684-116">Not supported.</span></span>|
|<span data-ttu-id="fe684-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe684-117">Application</span></span>|<span data-ttu-id="fe684-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe684-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe684-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe684-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fe684-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe684-120">Request headers</span></span>
|<span data-ttu-id="fe684-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe684-121">Header</span></span>|<span data-ttu-id="fe684-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fe684-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe684-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe684-123">Authorization</span></span>|<span data-ttu-id="fe684-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe684-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe684-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe684-125">Accept</span></span>|<span data-ttu-id="fe684-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe684-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe684-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe684-127">Request body</span></span>
<span data-ttu-id="fe684-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe684-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe684-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe684-129">Response</span></span>
<span data-ttu-id="fe684-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe684-130">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe684-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe684-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe684-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe684-132">Request</span></span>
<span data-ttu-id="fe684-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe684-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="fe684-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe684-134">Response</span></span>
<span data-ttu-id="fe684-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="fe684-135">Here is an example of the response.</span></span> <span data-ttu-id="fe684-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="fe684-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe684-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fe684-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2055

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeSuiteApp",
      "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
      "autoAcceptEula": true,
      "productIds": [
        "o365BusinessRetail"
      ],
      "excludedApps": {
        "@odata.type": "microsoft.graph.excludedApps",
        "access": true,
        "bing": true,
        "excel": true,
        "groove": true,
        "infoPath": true,
        "lync": true,
        "oneDrive": true,
        "oneNote": true,
        "outlook": true,
        "powerPoint": true,
        "publisher": true,
        "sharePointDesigner": true,
        "teams": true,
        "visio": true,
        "word": true
      },
      "useSharedComputerActivation": true,
      "updateChannel": "current",
      "officePlatformArchitecture": "x86",
      "localesToInstall": [
        "Locales To Install value"
      ],
      "installProgressDisplayLevel": "full",
      "shouldUninstallOlderVersionsOfOffice": true,
      "targetVersion": "Target Version value",
      "updateVersion": "Update Version value",
      "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
    }
  ]
}
```



