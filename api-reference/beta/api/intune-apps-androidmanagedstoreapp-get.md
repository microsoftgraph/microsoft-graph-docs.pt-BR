---
title: Obter androidManagedStoreApp
description: Leia as propriedades e os relacionamentos do objeto androidManagedStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b9a67ca7d71a25bddf217d8a115e8a2934aba728
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892247"
---
# <a name="get-androidmanagedstoreapp"></a><span data-ttu-id="28fd7-103">Obter androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="28fd7-103">Get androidManagedStoreApp</span></span>

> <span data-ttu-id="28fd7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="28fd7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28fd7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="28fd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28fd7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="28fd7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28fd7-107">Leia as propriedades e os relacionamentos do objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="28fd7-107">Read properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28fd7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28fd7-108">Prerequisites</span></span>
<span data-ttu-id="28fd7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28fd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28fd7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28fd7-111">Permission type</span></span>|<span data-ttu-id="28fd7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28fd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28fd7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28fd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28fd7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28fd7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="28fd7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28fd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28fd7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28fd7-116">Not supported.</span></span>|
|<span data-ttu-id="28fd7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28fd7-117">Application</span></span>|<span data-ttu-id="28fd7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28fd7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28fd7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28fd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28fd7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28fd7-120">Optional query parameters</span></span>
<span data-ttu-id="28fd7-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28fd7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="28fd7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28fd7-122">Request headers</span></span>
|<span data-ttu-id="28fd7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28fd7-123">Header</span></span>|<span data-ttu-id="28fd7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="28fd7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28fd7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="28fd7-125">Authorization</span></span>|<span data-ttu-id="28fd7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28fd7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28fd7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28fd7-127">Accept</span></span>|<span data-ttu-id="28fd7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="28fd7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28fd7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28fd7-129">Request body</span></span>
<span data-ttu-id="28fd7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28fd7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28fd7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="28fd7-131">Response</span></span>
<span data-ttu-id="28fd7-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28fd7-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28fd7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28fd7-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="28fd7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28fd7-134">Request</span></span>
<span data-ttu-id="28fd7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28fd7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="28fd7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="28fd7-136">Response</span></span>
<span data-ttu-id="28fd7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28fd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1037

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreApp",
    "id": "87247525-7525-8724-2575-248725752487",
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
    "packageId": "Package Id value",
    "appIdentifier": "App Identifier value",
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```





