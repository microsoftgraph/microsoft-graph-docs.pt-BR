---
title: Lista officeSuiteApps
description: Lista as propriedades e os relacionamentos dos objetos officeSuiteApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 173503a4ecef31b75ae0d2a4a1dc29b4f5de2d48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417417"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="f1034-103">Lista officeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="f1034-103">List officeSuiteApps</span></span>

> <span data-ttu-id="f1034-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1034-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1034-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1034-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1034-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f1034-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1034-107">Lista as propriedades e os relacionamentos dos objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f1034-107">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1034-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1034-108">Prerequisites</span></span>
<span data-ttu-id="f1034-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1034-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1034-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1034-111">Permission type</span></span>|<span data-ttu-id="f1034-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1034-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1034-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1034-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1034-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1034-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f1034-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1034-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1034-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1034-116">Not supported.</span></span>|
|<span data-ttu-id="f1034-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1034-117">Application</span></span>|<span data-ttu-id="f1034-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1034-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1034-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1034-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f1034-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1034-120">Request headers</span></span>
|<span data-ttu-id="f1034-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1034-121">Header</span></span>|<span data-ttu-id="f1034-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1034-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1034-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1034-123">Authorization</span></span>|<span data-ttu-id="f1034-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1034-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1034-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1034-125">Accept</span></span>|<span data-ttu-id="f1034-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1034-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1034-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1034-127">Request body</span></span>
<span data-ttu-id="f1034-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1034-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1034-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1034-129">Response</span></span>
<span data-ttu-id="f1034-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1034-130">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1034-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1034-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1034-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1034-132">Request</span></span>
<span data-ttu-id="f1034-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1034-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f1034-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1034-134">Response</span></span>
<span data-ttu-id="f1034-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1034-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

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
  ]
}
```




