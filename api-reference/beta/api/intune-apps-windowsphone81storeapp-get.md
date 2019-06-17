---
title: Obter windowsPhone81StoreApp
description: Leia as propriedades e as relações do objeto windowsPhone81StoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18823ffba7d0c67907e24c9e136bfe608ea3f2bf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972939"
---
# <a name="get-windowsphone81storeapp"></a><span data-ttu-id="b64ae-103">Obter windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="b64ae-103">Get windowsPhone81StoreApp</span></span>

> <span data-ttu-id="b64ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b64ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b64ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b64ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b64ae-106">Leia as propriedades e as relações do objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b64ae-106">Read properties and relationships of the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b64ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b64ae-107">Prerequisites</span></span>
<span data-ttu-id="b64ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b64ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b64ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b64ae-110">Permission type</span></span>|<span data-ttu-id="b64ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b64ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b64ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b64ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b64ae-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b64ae-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b64ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b64ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b64ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b64ae-115">Not supported.</span></span>|
|<span data-ttu-id="b64ae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b64ae-116">Application</span></span>|<span data-ttu-id="b64ae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b64ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b64ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b64ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b64ae-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b64ae-119">Optional query parameters</span></span>
<span data-ttu-id="b64ae-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b64ae-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b64ae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b64ae-121">Request headers</span></span>
|<span data-ttu-id="b64ae-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b64ae-122">Header</span></span>|<span data-ttu-id="b64ae-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b64ae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b64ae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b64ae-124">Authorization</span></span>|<span data-ttu-id="b64ae-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b64ae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b64ae-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b64ae-126">Accept</span></span>|<span data-ttu-id="b64ae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b64ae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b64ae-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b64ae-128">Request body</span></span>
<span data-ttu-id="b64ae-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b64ae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b64ae-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b64ae-130">Response</span></span>
<span data-ttu-id="b64ae-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b64ae-131">If successful, this method returns a `200 OK` response code and [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b64ae-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b64ae-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b64ae-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b64ae-133">Request</span></span>
<span data-ttu-id="b64ae-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b64ae-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b64ae-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b64ae-135">Response</span></span>
<span data-ttu-id="b64ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b64ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1018

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
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```





