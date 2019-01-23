---
title: Listar iosLobApps
description: Listar propriedades e relações dos objetos iosLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 259f90a990b4ada50ae2106bddf266d16a30e76b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421519"
---
# <a name="list-ioslobapps"></a><span data-ttu-id="38c41-103">Listar iosLobApps</span><span class="sxs-lookup"><span data-stu-id="38c41-103">List iosLobApps</span></span>

> <span data-ttu-id="38c41-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="38c41-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38c41-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38c41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38c41-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="38c41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38c41-107">Listar propriedades e relações dos objetos [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="38c41-107">List properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38c41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38c41-108">Prerequisites</span></span>
<span data-ttu-id="38c41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="38c41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="38c41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38c41-111">Permission type</span></span>|<span data-ttu-id="38c41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38c41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38c41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38c41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38c41-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="38c41-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="38c41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38c41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38c41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38c41-116">Not supported.</span></span>|
|<span data-ttu-id="38c41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38c41-117">Application</span></span>|<span data-ttu-id="38c41-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38c41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38c41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38c41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="38c41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38c41-120">Request headers</span></span>
|<span data-ttu-id="38c41-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38c41-121">Header</span></span>|<span data-ttu-id="38c41-122">Valor</span><span class="sxs-lookup"><span data-stu-id="38c41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38c41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="38c41-123">Authorization</span></span>|<span data-ttu-id="38c41-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38c41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38c41-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38c41-125">Accept</span></span>|<span data-ttu-id="38c41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38c41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38c41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38c41-127">Request body</span></span>
<span data-ttu-id="38c41-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38c41-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38c41-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="38c41-129">Response</span></span>
<span data-ttu-id="38c41-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38c41-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobApp](../resources/intune-apps-ioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38c41-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38c41-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="38c41-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38c41-132">Request</span></span>
<span data-ttu-id="38c41-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38c41-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="38c41-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="38c41-134">Response</span></span>
<span data-ttu-id="38c41-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38c41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1749

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobApp",
      "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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




