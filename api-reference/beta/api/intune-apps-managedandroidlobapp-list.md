---
title: Listar managedAndroidLobApps
description: Listar propriedades e relações dos objetos managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7954b7b7204de0690de4415a21dec83a3836bc76
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157299"
---
# <a name="list-managedandroidlobapps"></a><span data-ttu-id="b91c2-103">Listar managedAndroidLobApps</span><span class="sxs-lookup"><span data-stu-id="b91c2-103">List managedAndroidLobApps</span></span>

<span data-ttu-id="b91c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b91c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b91c2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b91c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b91c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b91c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b91c2-107">Listar propriedades e relações dos objetos [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b91c2-107">List properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b91c2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b91c2-108">Prerequisites</span></span>
<span data-ttu-id="b91c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b91c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b91c2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b91c2-111">Permission type</span></span>|<span data-ttu-id="b91c2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b91c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b91c2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b91c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b91c2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b91c2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b91c2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b91c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b91c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b91c2-116">Not supported.</span></span>|
|<span data-ttu-id="b91c2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b91c2-117">Application</span></span>|<span data-ttu-id="b91c2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b91c2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b91c2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b91c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b91c2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b91c2-120">Request headers</span></span>
|<span data-ttu-id="b91c2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b91c2-121">Header</span></span>|<span data-ttu-id="b91c2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b91c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b91c2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b91c2-123">Authorization</span></span>|<span data-ttu-id="b91c2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b91c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b91c2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b91c2-125">Accept</span></span>|<span data-ttu-id="b91c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b91c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b91c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b91c2-127">Request body</span></span>
<span data-ttu-id="b91c2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b91c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b91c2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b91c2-129">Response</span></span>
<span data-ttu-id="b91c2-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b91c2-130">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b91c2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b91c2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b91c2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b91c2-132">Request</span></span>
<span data-ttu-id="b91c2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b91c2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="b91c2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b91c2-134">Response</span></span>
<span data-ttu-id="b91c2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b91c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2017

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAndroidLobApp",
      "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "packageId": "Package Id value",
      "identityName": "Identity Name value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
        "v4_0": true,
        "v4_0_3": true,
        "v4_1": true,
        "v4_2": true,
        "v4_3": true,
        "v4_4": true,
        "v5_0": true,
        "v5_1": true,
        "v6_0": true,
        "v7_0": true,
        "v7_1": true,
        "v8_0": true,
        "v8_1": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true
      },
      "versionName": "Version Name value",
      "versionCode": "Version Code value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```




