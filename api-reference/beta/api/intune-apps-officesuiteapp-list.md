---
title: Listar officeSuiteApps
description: Listar Propriedades e relações dos objetos officeSuiteApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dbed55882a75af4c731c8e7c5e4113dbb206e85d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444900"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="4b6e0-103">Listar officeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="4b6e0-103">List officeSuiteApps</span></span>

<span data-ttu-id="4b6e0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b6e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b6e0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b6e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b6e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b6e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b6e0-107">Listar Propriedades e relações dos objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4b6e0-107">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b6e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b6e0-108">Prerequisites</span></span>
<span data-ttu-id="4b6e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b6e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b6e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b6e0-111">Permission type</span></span>|<span data-ttu-id="4b6e0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b6e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b6e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b6e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b6e0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b6e0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4b6e0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b6e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b6e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b6e0-116">Not supported.</span></span>|
|<span data-ttu-id="4b6e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b6e0-117">Application</span></span>|<span data-ttu-id="4b6e0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b6e0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b6e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b6e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4b6e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b6e0-120">Request headers</span></span>
|<span data-ttu-id="4b6e0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b6e0-121">Header</span></span>|<span data-ttu-id="4b6e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b6e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b6e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b6e0-123">Authorization</span></span>|<span data-ttu-id="4b6e0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b6e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b6e0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b6e0-125">Accept</span></span>|<span data-ttu-id="4b6e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b6e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b6e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b6e0-127">Request body</span></span>
<span data-ttu-id="4b6e0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b6e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b6e0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b6e0-129">Response</span></span>
<span data-ttu-id="4b6e0-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b6e0-130">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b6e0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b6e0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b6e0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b6e0-132">Request</span></span>
<span data-ttu-id="4b6e0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b6e0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="4b6e0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b6e0-134">Response</span></span>
<span data-ttu-id="4b6e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b6e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2032

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





