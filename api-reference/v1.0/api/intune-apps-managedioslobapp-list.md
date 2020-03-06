---
title: Listar managedIOSLobApps
description: Listar propriedades e relações dos objetos managedIOSLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e3473521559d8020c79672db4d28920dbe83d5b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516177"
---
# <a name="list-managedioslobapps"></a><span data-ttu-id="86e51-103">Listar managedIOSLobApps</span><span class="sxs-lookup"><span data-stu-id="86e51-103">List managedIOSLobApps</span></span>

<span data-ttu-id="86e51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86e51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86e51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86e51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86e51-106">Listar propriedades e relações dos objetos [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="86e51-106">List properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86e51-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86e51-107">Prerequisites</span></span>
<span data-ttu-id="86e51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="86e51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="86e51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86e51-110">Permission type</span></span>|<span data-ttu-id="86e51-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86e51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86e51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86e51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86e51-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86e51-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86e51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86e51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86e51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86e51-115">Not supported.</span></span>|
|<span data-ttu-id="86e51-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86e51-116">Application</span></span>|<span data-ttu-id="86e51-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86e51-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86e51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86e51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="86e51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86e51-119">Request headers</span></span>
|<span data-ttu-id="86e51-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86e51-120">Header</span></span>|<span data-ttu-id="86e51-121">Valor</span><span class="sxs-lookup"><span data-stu-id="86e51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86e51-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86e51-122">Authorization</span></span>|<span data-ttu-id="86e51-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86e51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86e51-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86e51-124">Accept</span></span>|<span data-ttu-id="86e51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86e51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86e51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86e51-126">Request body</span></span>
<span data-ttu-id="86e51-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86e51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86e51-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="86e51-128">Response</span></span>
<span data-ttu-id="86e51-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86e51-129">If successful, this method returns a `200 OK` response code and a collection of [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86e51-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86e51-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="86e51-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86e51-131">Request</span></span>
<span data-ttu-id="86e51-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86e51-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="86e51-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="86e51-133">Response</span></span>
<span data-ttu-id="86e51-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86e51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1680

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
        "v12_0": true,
        "v13_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value"
    }
  ]
}
```




