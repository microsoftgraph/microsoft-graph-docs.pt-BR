---
title: Listar managedIOSLobApps
description: Listar propriedades e relações dos objetos managedIOSLobApp.
author: tfitzmac
ms.openlocfilehash: f3a2d3cae0e3b07d4e8b79ead2a85bc2aa7469ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340338"
---
# <a name="list-managedioslobapps"></a><span data-ttu-id="20fad-103">Listar managedIOSLobApps</span><span class="sxs-lookup"><span data-stu-id="20fad-103">List managedIOSLobApps</span></span>

> <span data-ttu-id="20fad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20fad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20fad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20fad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20fad-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="20fad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20fad-107">Listar propriedades e relações dos objetos [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="20fad-107">List properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20fad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20fad-108">Prerequisites</span></span>
<span data-ttu-id="20fad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20fad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20fad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20fad-111">Permission type</span></span>|<span data-ttu-id="20fad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20fad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20fad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20fad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20fad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="20fad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="20fad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20fad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20fad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20fad-116">Not supported.</span></span>|
|<span data-ttu-id="20fad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20fad-117">Application</span></span>|<span data-ttu-id="20fad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20fad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20fad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20fad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="20fad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20fad-120">Request headers</span></span>
|<span data-ttu-id="20fad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20fad-121">Header</span></span>|<span data-ttu-id="20fad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="20fad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20fad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20fad-123">Authorization</span></span>|<span data-ttu-id="20fad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20fad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20fad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20fad-125">Accept</span></span>|<span data-ttu-id="20fad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20fad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20fad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20fad-127">Request body</span></span>
<span data-ttu-id="20fad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20fad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20fad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="20fad-129">Response</span></span>
<span data-ttu-id="20fad-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20fad-130">If successful, this method returns a `200 OK` response code and a collection of [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20fad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20fad-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="20fad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20fad-132">Request</span></span>
<span data-ttu-id="20fad-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20fad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="20fad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="20fad-134">Response</span></span>
<span data-ttu-id="20fad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20fad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1734

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSLobApp",
      "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "bundleId": "Bundle Id value",
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
        "v8_0": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true,
        "v12_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```





