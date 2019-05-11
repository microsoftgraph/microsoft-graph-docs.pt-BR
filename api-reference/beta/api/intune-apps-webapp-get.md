---
title: Acessar webApp
description: Leia as propriedades e as relações do objeto webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a02d1aac676b0039427685c530b72781fa2e745b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934849"
---
# <a name="get-webapp"></a><span data-ttu-id="b07ab-103">Acessar webApp</span><span class="sxs-lookup"><span data-stu-id="b07ab-103">Get webApp</span></span>

> <span data-ttu-id="b07ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b07ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b07ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b07ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b07ab-106">Leia as propriedades e as relações do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="b07ab-106">Read properties and relationships of the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b07ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b07ab-107">Prerequisites</span></span>
<span data-ttu-id="b07ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b07ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b07ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b07ab-110">Permission type</span></span>|<span data-ttu-id="b07ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b07ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b07ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b07ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b07ab-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07ab-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b07ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b07ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b07ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b07ab-115">Not supported.</span></span>|
|<span data-ttu-id="b07ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b07ab-116">Application</span></span>|<span data-ttu-id="b07ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b07ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b07ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b07ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b07ab-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b07ab-119">Optional query parameters</span></span>
<span data-ttu-id="b07ab-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b07ab-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b07ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b07ab-121">Request headers</span></span>
|<span data-ttu-id="b07ab-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b07ab-122">Header</span></span>|<span data-ttu-id="b07ab-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b07ab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b07ab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b07ab-124">Authorization</span></span>|<span data-ttu-id="b07ab-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b07ab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b07ab-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b07ab-126">Accept</span></span>|<span data-ttu-id="b07ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b07ab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b07ab-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b07ab-128">Request body</span></span>
<span data-ttu-id="b07ab-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b07ab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b07ab-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b07ab-130">Response</span></span>
<span data-ttu-id="b07ab-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b07ab-131">If successful, this method returns a `200 OK` response code and [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b07ab-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b07ab-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b07ab-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b07ab-133">Request</span></span>
<span data-ttu-id="b07ab-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b07ab-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b07ab-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b07ab-135">Response</span></span>
<span data-ttu-id="b07ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b07ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1024

{
  "value": {
    "@odata.type": "#microsoft.graph.webApp",
    "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
    "appUrl": "https://example.com/appUrl/",
    "useManagedBrowser": true
  }
}
```




