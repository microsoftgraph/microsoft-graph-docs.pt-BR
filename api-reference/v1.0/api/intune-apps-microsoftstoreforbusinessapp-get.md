---
title: Get microsoftStoreForBusinessApp
description: Ler propriedades e relações do objeto microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea390278b0e942e17681c4dcf1bd06f3ad55ccec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262689"
---
# <a name="get-microsoftstoreforbusinessapp"></a><span data-ttu-id="759d1-103">Get microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="759d1-103">Get microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="759d1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="759d1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="759d1-105">Ler propriedades e relações do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="759d1-105">Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="759d1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="759d1-106">Prerequisites</span></span>
<span data-ttu-id="759d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="759d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="759d1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="759d1-109">Permission type</span></span>|<span data-ttu-id="759d1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="759d1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="759d1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="759d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="759d1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="759d1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="759d1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="759d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="759d1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="759d1-114">Not supported.</span></span>|
|<span data-ttu-id="759d1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="759d1-115">Application</span></span>|<span data-ttu-id="759d1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="759d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="759d1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="759d1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="759d1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="759d1-118">Optional query parameters</span></span>
<span data-ttu-id="759d1-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="759d1-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="759d1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="759d1-120">Request headers</span></span>
|<span data-ttu-id="759d1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="759d1-121">Header</span></span>|<span data-ttu-id="759d1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="759d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="759d1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="759d1-123">Authorization</span></span>|<span data-ttu-id="759d1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="759d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="759d1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="759d1-125">Accept</span></span>|<span data-ttu-id="759d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="759d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="759d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="759d1-127">Request body</span></span>
<span data-ttu-id="759d1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="759d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="759d1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="759d1-129">Response</span></span>
<span data-ttu-id="759d1-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="759d1-130">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="759d1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="759d1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="759d1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="759d1-132">Request</span></span>
<span data-ttu-id="759d1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="759d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="759d1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="759d1-134">Response</span></span>
<span data-ttu-id="759d1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="759d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



