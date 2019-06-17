---
title: Acessar mobileApp
description: Leia as propriedades e as relações do objeto mobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22527f05404dd3857ef41151760d66e7d8e5883b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974290"
---
# <a name="get-mobileapp"></a><span data-ttu-id="8ed67-103">Acessar mobileApp</span><span class="sxs-lookup"><span data-stu-id="8ed67-103">Get mobileApp</span></span>

> <span data-ttu-id="8ed67-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ed67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ed67-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ed67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ed67-106">Leia as propriedades e as relações do objeto [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ed67-106">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ed67-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ed67-107">Prerequisites</span></span>
<span data-ttu-id="8ed67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ed67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ed67-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ed67-110">Permission type</span></span>|<span data-ttu-id="8ed67-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ed67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ed67-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ed67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ed67-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ed67-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8ed67-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ed67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ed67-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ed67-115">Not supported.</span></span>|
|<span data-ttu-id="8ed67-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ed67-116">Application</span></span>|<span data-ttu-id="8ed67-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ed67-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ed67-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ed67-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ed67-119">Optional query parameters</span></span>
<span data-ttu-id="8ed67-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed67-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ed67-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed67-121">Request headers</span></span>
|<span data-ttu-id="8ed67-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ed67-122">Header</span></span>|<span data-ttu-id="8ed67-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8ed67-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ed67-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ed67-124">Authorization</span></span>|<span data-ttu-id="8ed67-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ed67-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ed67-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ed67-126">Accept</span></span>|<span data-ttu-id="8ed67-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8ed67-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ed67-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed67-128">Request body</span></span>
<span data-ttu-id="8ed67-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ed67-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ed67-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed67-130">Response</span></span>
<span data-ttu-id="8ed67-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileApp](../resources/intune-apps-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed67-131">If successful, this method returns a `200 OK` response code and [mobileApp](../resources/intune-apps-mobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ed67-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ed67-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ed67-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed67-133">Request</span></span>
<span data-ttu-id="8ed67-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ed67-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="8ed67-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed67-135">Response</span></span>
<span data-ttu-id="8ed67-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ed67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 949

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileApp",
    "id": "0177548a-548a-0177-8a54-77018a547701",
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
    "dependentAppCount": 1
  }
}
```





