---
title: Lista officeSuiteApps
description: Lista as propriedades e os relacionamentos dos objetos officeSuiteApp.
author: tfitzmac
ms.openlocfilehash: 2b6366da8bf36954fedaa9670f0de71ed723c06c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350663"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="3a88f-103">Lista officeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="3a88f-103">List officeSuiteApps</span></span>

> <span data-ttu-id="3a88f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a88f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a88f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a88f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a88f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3a88f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a88f-107">Lista as propriedades e os relacionamentos dos objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3a88f-107">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a88f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a88f-108">Prerequisites</span></span>
<span data-ttu-id="3a88f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a88f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a88f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a88f-111">Permission type</span></span>|<span data-ttu-id="3a88f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a88f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a88f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a88f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a88f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a88f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3a88f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a88f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a88f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a88f-116">Not supported.</span></span>|
|<span data-ttu-id="3a88f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a88f-117">Application</span></span>|<span data-ttu-id="3a88f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a88f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a88f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a88f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3a88f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a88f-120">Request headers</span></span>
|<span data-ttu-id="3a88f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a88f-121">Header</span></span>|<span data-ttu-id="3a88f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3a88f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a88f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a88f-123">Authorization</span></span>|<span data-ttu-id="3a88f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a88f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a88f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a88f-125">Accept</span></span>|<span data-ttu-id="3a88f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a88f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a88f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a88f-127">Request body</span></span>
<span data-ttu-id="3a88f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a88f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a88f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a88f-129">Response</span></span>
<span data-ttu-id="3a88f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a88f-130">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a88f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a88f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a88f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a88f-132">Request</span></span>
<span data-ttu-id="3a88f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a88f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="3a88f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a88f-134">Response</span></span>
<span data-ttu-id="3a88f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a88f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1807

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
      "updateVersion": "Update Version value"
    }
  ]
}
```





