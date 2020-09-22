---
title: Listar androidForWorkApps
description: Listar Propriedades e relações dos objetos androidForWorkApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c048895c3c82ddc8cec0aeca8187d6c2d4177d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006521"
---
# <a name="list-androidforworkapps"></a><span data-ttu-id="ec89a-103">Listar androidForWorkApps</span><span class="sxs-lookup"><span data-stu-id="ec89a-103">List androidForWorkApps</span></span>

<span data-ttu-id="ec89a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec89a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec89a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec89a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec89a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec89a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec89a-107">Listar Propriedades e relações dos objetos [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ec89a-107">List properties and relationships of the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec89a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec89a-108">Prerequisites</span></span>
<span data-ttu-id="ec89a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec89a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec89a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec89a-111">Permission type</span></span>|<span data-ttu-id="ec89a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec89a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec89a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec89a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec89a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec89a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ec89a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec89a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec89a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec89a-116">Not supported.</span></span>|
|<span data-ttu-id="ec89a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec89a-117">Application</span></span>|<span data-ttu-id="ec89a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec89a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec89a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec89a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ec89a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec89a-120">Request headers</span></span>
|<span data-ttu-id="ec89a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec89a-121">Header</span></span>|<span data-ttu-id="ec89a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ec89a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec89a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec89a-123">Authorization</span></span>|<span data-ttu-id="ec89a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec89a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec89a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec89a-125">Accept</span></span>|<span data-ttu-id="ec89a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec89a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec89a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec89a-127">Request body</span></span>
<span data-ttu-id="ec89a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec89a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec89a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec89a-129">Response</span></span>
<span data-ttu-id="ec89a-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec89a-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec89a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec89a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec89a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec89a-132">Request</span></span>
<span data-ttu-id="ec89a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec89a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="ec89a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec89a-134">Response</span></span>
<span data-ttu-id="ec89a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec89a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1293

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkApp",
      "id": "c5010785-0785-c501-8507-01c5850701c5",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/"
    }
  ]
}
```






