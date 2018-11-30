---
title: Obter androidManagedStoreApp
description: Leia as propriedades e os relacionamentos do objeto androidManagedStoreApp.
ms.openlocfilehash: 2315a9757934019e7fae238c6d0f7f11bec1544a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035525"
---
# <a name="get-androidmanagedstoreapp"></a><span data-ttu-id="f58aa-103">Obter androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="f58aa-103">Get androidManagedStoreApp</span></span>

> <span data-ttu-id="f58aa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f58aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f58aa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f58aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f58aa-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f58aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f58aa-107">Leia as propriedades e os relacionamentos do objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f58aa-107">Read properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f58aa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f58aa-108">Prerequisites</span></span>
<span data-ttu-id="f58aa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f58aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f58aa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f58aa-111">Permission type</span></span>|<span data-ttu-id="f58aa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f58aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f58aa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f58aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f58aa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f58aa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f58aa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f58aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f58aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f58aa-116">Not supported.</span></span>|
|<span data-ttu-id="f58aa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f58aa-117">Application</span></span>|<span data-ttu-id="f58aa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f58aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f58aa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f58aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f58aa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f58aa-120">Optional query parameters</span></span>
<span data-ttu-id="f58aa-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f58aa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f58aa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f58aa-122">Request headers</span></span>
|<span data-ttu-id="f58aa-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f58aa-123">Header</span></span>|<span data-ttu-id="f58aa-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f58aa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f58aa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f58aa-125">Authorization</span></span>|<span data-ttu-id="f58aa-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f58aa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f58aa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f58aa-127">Accept</span></span>|<span data-ttu-id="f58aa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f58aa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f58aa-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f58aa-129">Request body</span></span>
<span data-ttu-id="f58aa-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f58aa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f58aa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f58aa-131">Response</span></span>
<span data-ttu-id="f58aa-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f58aa-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f58aa-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f58aa-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f58aa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f58aa-134">Request</span></span>
<span data-ttu-id="f58aa-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f58aa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f58aa-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f58aa-136">Response</span></span>
<span data-ttu-id="f58aa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f58aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





