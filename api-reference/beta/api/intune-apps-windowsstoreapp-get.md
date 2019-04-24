---
title: Obter windowsStoreApp
description: Leia as propriedades e as relações do objeto windowsStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a723b135a8d0b315db9b3c84fe561c38cc01d59a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32486087"
---
# <a name="get-windowsstoreapp"></a><span data-ttu-id="f448c-103">Obter windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="f448c-103">Get windowsStoreApp</span></span>

> <span data-ttu-id="f448c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f448c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f448c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f448c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f448c-106">Leia as propriedades e as relações do objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f448c-106">Read properties and relationships of the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f448c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f448c-107">Prerequisites</span></span>
<span data-ttu-id="f448c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f448c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f448c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f448c-110">Permission type</span></span>|<span data-ttu-id="f448c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f448c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f448c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f448c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f448c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f448c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f448c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f448c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f448c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f448c-115">Not supported.</span></span>|
|<span data-ttu-id="f448c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f448c-116">Application</span></span>|<span data-ttu-id="f448c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f448c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f448c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f448c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f448c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f448c-119">Optional query parameters</span></span>
<span data-ttu-id="f448c-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f448c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f448c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f448c-121">Request headers</span></span>
|<span data-ttu-id="f448c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f448c-122">Header</span></span>|<span data-ttu-id="f448c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f448c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f448c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f448c-124">Authorization</span></span>|<span data-ttu-id="f448c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f448c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f448c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f448c-126">Accept</span></span>|<span data-ttu-id="f448c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f448c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f448c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f448c-128">Request body</span></span>
<span data-ttu-id="f448c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f448c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f448c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f448c-130">Response</span></span>
<span data-ttu-id="f448c-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f448c-131">If successful, this method returns a `200 OK` response code and [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f448c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f448c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f448c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f448c-133">Request</span></span>
<span data-ttu-id="f448c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f448c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f448c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f448c-135">Response</span></span>
<span data-ttu-id="f448c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f448c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1011

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsStoreApp",
    "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```





