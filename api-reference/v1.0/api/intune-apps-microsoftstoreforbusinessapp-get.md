---
title: Get microsoftStoreForBusinessApp
description: Ler propriedades e relações do objeto microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03eb9f682bbcc37ee81cdbec43773a98f8326301
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759760"
---
# <a name="get-microsoftstoreforbusinessapp"></a><span data-ttu-id="f2e4b-103">Get microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="f2e4b-103">Get microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="f2e4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2e4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2e4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2e4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2e4b-106">Ler propriedades e relações do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2e4b-106">Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2e4b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2e4b-107">Prerequisites</span></span>
<span data-ttu-id="f2e4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2e4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2e4b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2e4b-110">Permission type</span></span>|<span data-ttu-id="f2e4b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2e4b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2e4b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2e4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2e4b-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e4b-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2e4b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2e4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2e4b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2e4b-115">Not supported.</span></span>|
|<span data-ttu-id="f2e4b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2e4b-116">Application</span></span>|<span data-ttu-id="f2e4b-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e4b-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2e4b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2e4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2e4b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2e4b-119">Optional query parameters</span></span>
<span data-ttu-id="f2e4b-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2e4b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2e4b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e4b-121">Request headers</span></span>
|<span data-ttu-id="f2e4b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2e4b-122">Header</span></span>|<span data-ttu-id="f2e4b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f2e4b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2e4b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2e4b-124">Authorization</span></span>|<span data-ttu-id="f2e4b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2e4b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2e4b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2e4b-126">Accept</span></span>|<span data-ttu-id="f2e4b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f2e4b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2e4b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e4b-128">Request body</span></span>
<span data-ttu-id="f2e4b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2e4b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2e4b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2e4b-130">Response</span></span>
<span data-ttu-id="f2e4b-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2e4b-131">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e4b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2e4b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2e4b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2e4b-133">Request</span></span>
<span data-ttu-id="f2e4b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2e4b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f2e4b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2e4b-135">Response</span></span>
<span data-ttu-id="f2e4b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2e4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1008

{
  "value": {
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
}
```




