---
title: Listar microsoftStoreForBusinessApps
description: Listar propriedades e relações dos objetos microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 25197e9b2387a2691241d1b2c99187657f6579c5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139976"
---
# <a name="list-microsoftstoreforbusinessapps"></a><span data-ttu-id="8dfef-103">Listar microsoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="8dfef-103">List microsoftStoreForBusinessApps</span></span>

<span data-ttu-id="8dfef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dfef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dfef-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8dfef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dfef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8dfef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dfef-107">Listar propriedades e relações dos objetos [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dfef-107">List properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dfef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8dfef-108">Prerequisites</span></span>
<span data-ttu-id="8dfef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dfef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dfef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dfef-111">Permission type</span></span>|<span data-ttu-id="8dfef-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8dfef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dfef-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dfef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8dfef-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dfef-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8dfef-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dfef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dfef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dfef-116">Not supported.</span></span>|
|<span data-ttu-id="8dfef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dfef-117">Application</span></span>|<span data-ttu-id="8dfef-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dfef-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dfef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dfef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8dfef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dfef-120">Request headers</span></span>
|<span data-ttu-id="8dfef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8dfef-121">Header</span></span>|<span data-ttu-id="8dfef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8dfef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dfef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8dfef-123">Authorization</span></span>|<span data-ttu-id="8dfef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dfef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dfef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8dfef-125">Accept</span></span>|<span data-ttu-id="8dfef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8dfef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dfef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dfef-127">Request body</span></span>
<span data-ttu-id="8dfef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8dfef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dfef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dfef-129">Response</span></span>
<span data-ttu-id="8dfef-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dfef-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dfef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dfef-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dfef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dfef-132">Request</span></span>
<span data-ttu-id="8dfef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dfef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="8dfef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dfef-134">Response</span></span>
<span data-ttu-id="8dfef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dfef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1550

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
      "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "productKey": "Product Key value",
      "licenseType": "online",
      "packageIdentityName": "Package Identity Name value",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportUserLicensing": true,
        "supportDeviceLicensing": true,
        "supportsUserLicensing": true,
        "supportsDeviceLicensing": true
      }
    }
  ]
}
```




