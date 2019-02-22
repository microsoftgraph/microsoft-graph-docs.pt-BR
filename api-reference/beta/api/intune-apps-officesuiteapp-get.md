---
title: Obter officeSuiteApp
description: Leia as propriedades e as relações do objeto officeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7417c55fc05d808b9b071e96eb412a4f296d1c9a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159602"
---
# <a name="get-officesuiteapp"></a><span data-ttu-id="e4748-103">Obter officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="e4748-103">Get officeSuiteApp</span></span>

> <span data-ttu-id="e4748-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4748-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4748-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4748-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4748-106">Leia as propriedades e as relações do objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e4748-106">Read properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4748-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4748-107">Prerequisites</span></span>
<span data-ttu-id="e4748-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e4748-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4748-110">Permission type</span></span>|<span data-ttu-id="e4748-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4748-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4748-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4748-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4748-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4748-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e4748-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4748-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4748-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4748-115">Not supported.</span></span>|
|<span data-ttu-id="e4748-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4748-116">Application</span></span>|<span data-ttu-id="e4748-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4748-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4748-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4748-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4748-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e4748-119">Optional query parameters</span></span>
<span data-ttu-id="e4748-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e4748-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4748-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4748-121">Request headers</span></span>
|<span data-ttu-id="e4748-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4748-122">Header</span></span>|<span data-ttu-id="e4748-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e4748-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4748-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4748-124">Authorization</span></span>|<span data-ttu-id="e4748-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4748-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4748-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4748-126">Accept</span></span>|<span data-ttu-id="e4748-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e4748-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4748-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4748-128">Request body</span></span>
<span data-ttu-id="e4748-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4748-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4748-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4748-130">Response</span></span>
<span data-ttu-id="e4748-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4748-131">If successful, this method returns a `200 OK` response code and [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4748-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4748-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4748-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4748-133">Request</span></span>
<span data-ttu-id="e4748-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4748-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e4748-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4748-135">Response</span></span>
<span data-ttu-id="e4748-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4748-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1853

{
  "value": {
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
}
```




