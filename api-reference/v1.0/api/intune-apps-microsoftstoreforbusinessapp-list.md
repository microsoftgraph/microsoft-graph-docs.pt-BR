---
title: Listar microsoftStoreForBusinessApps
description: Listar propriedades e relações dos objetos microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75ba83073715b99903bda0388876a511233de243
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754137"
---
# <a name="list-microsoftstoreforbusinessapps"></a><span data-ttu-id="1b185-103">Listar microsoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="1b185-103">List microsoftStoreForBusinessApps</span></span>

<span data-ttu-id="1b185-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b185-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b185-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b185-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b185-106">Listar propriedades e relações dos objetos [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b185-106">List properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b185-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b185-107">Prerequisites</span></span>
<span data-ttu-id="1b185-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b185-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b185-110">Permission type</span></span>|<span data-ttu-id="1b185-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b185-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b185-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b185-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b185-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b185-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b185-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b185-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b185-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b185-115">Not supported.</span></span>|
|<span data-ttu-id="1b185-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b185-116">Application</span></span>|<span data-ttu-id="1b185-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b185-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b185-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b185-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1b185-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b185-119">Request headers</span></span>
|<span data-ttu-id="1b185-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b185-120">Header</span></span>|<span data-ttu-id="1b185-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1b185-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b185-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b185-122">Authorization</span></span>|<span data-ttu-id="1b185-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b185-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b185-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b185-124">Accept</span></span>|<span data-ttu-id="1b185-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b185-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b185-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b185-126">Request body</span></span>
<span data-ttu-id="1b185-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b185-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b185-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b185-128">Response</span></span>
<span data-ttu-id="1b185-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b185-129">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b185-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b185-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b185-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b185-131">Request</span></span>
<span data-ttu-id="1b185-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b185-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="1b185-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b185-133">Response</span></span>
<span data-ttu-id="1b185-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b185-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1070

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
      "publishingState": "processing",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "productKey": "Product Key value",
      "licenseType": "online",
      "packageIdentityName": "Package Identity Name value"
    }
  ]
}
```




