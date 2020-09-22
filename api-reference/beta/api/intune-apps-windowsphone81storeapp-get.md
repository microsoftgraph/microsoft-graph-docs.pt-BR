---
title: Obter windowsPhone81StoreApp
description: Leia as propriedades e as relações do objeto windowsPhone81StoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a8fa07147d47357d353fbc1a763a5966dfc45538
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976267"
---
# <a name="get-windowsphone81storeapp"></a><span data-ttu-id="e8f2a-103">Obter windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="e8f2a-103">Get windowsPhone81StoreApp</span></span>

<span data-ttu-id="e8f2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8f2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8f2a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8f2a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8f2a-107">Leia as propriedades e as relações do objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e8f2a-107">Read properties and relationships of the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8f2a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8f2a-108">Prerequisites</span></span>
<span data-ttu-id="e8f2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8f2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8f2a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8f2a-111">Permission type</span></span>|<span data-ttu-id="e8f2a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8f2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8f2a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8f2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8f2a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8f2a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e8f2a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8f2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8f2a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-116">Not supported.</span></span>|
|<span data-ttu-id="e8f2a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8f2a-117">Application</span></span>|<span data-ttu-id="e8f2a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8f2a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8f2a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8f2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8f2a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8f2a-120">Optional query parameters</span></span>
<span data-ttu-id="e8f2a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8f2a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f2a-122">Request headers</span></span>
|<span data-ttu-id="e8f2a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8f2a-123">Header</span></span>|<span data-ttu-id="e8f2a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e8f2a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8f2a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8f2a-125">Authorization</span></span>|<span data-ttu-id="e8f2a-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8f2a-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8f2a-127">Accept</span></span>|<span data-ttu-id="e8f2a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e8f2a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8f2a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f2a-129">Request body</span></span>
<span data-ttu-id="e8f2a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8f2a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8f2a-131">Response</span></span>
<span data-ttu-id="e8f2a-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-132">If successful, this method returns a `200 OK` response code and [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8f2a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8f2a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8f2a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f2a-134">Request</span></span>
<span data-ttu-id="e8f2a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e8f2a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8f2a-136">Response</span></span>
<span data-ttu-id="e8f2a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8f2a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1079

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
    "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```






