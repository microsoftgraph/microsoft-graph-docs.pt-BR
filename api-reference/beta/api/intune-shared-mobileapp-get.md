---
title: Acessar mobileApp
description: Leia as propriedades e as relações do objeto mobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0010bcd664700b3fa11171ec33738f17fafc506c
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538011"
---
# <a name="get-mobileapp"></a><span data-ttu-id="2ef46-103">Acessar mobileApp</span><span class="sxs-lookup"><span data-stu-id="2ef46-103">Get mobileApp</span></span>

> <span data-ttu-id="2ef46-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ef46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ef46-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ef46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ef46-106">Leia as propriedades e as relações do objeto [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ef46-106">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ef46-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ef46-107">Prerequisites</span></span>
<span data-ttu-id="2ef46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef46-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ef46-110">Permission type</span></span>|<span data-ttu-id="2ef46-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ef46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ef46-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ef46-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2ef46-113">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="2ef46-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="2ef46-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ef46-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="2ef46-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="2ef46-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2ef46-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ef46-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2ef46-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ef46-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ef46-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef46-118">Not supported.</span></span>|
|<span data-ttu-id="2ef46-119">Application</span><span class="sxs-lookup"><span data-stu-id="2ef46-119">Application</span></span>||
| <span data-ttu-id="2ef46-120">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="2ef46-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="2ef46-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ef46-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="2ef46-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="2ef46-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2ef46-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ef46-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ef46-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef46-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ef46-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ef46-125">Optional query parameters</span></span>
<span data-ttu-id="2ef46-126">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef46-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ef46-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef46-127">Request headers</span></span>
|<span data-ttu-id="2ef46-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ef46-128">Header</span></span>|<span data-ttu-id="2ef46-129">Valor</span><span class="sxs-lookup"><span data-stu-id="2ef46-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ef46-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ef46-130">Authorization</span></span>|<span data-ttu-id="2ef46-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ef46-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ef46-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ef46-132">Accept</span></span>|<span data-ttu-id="2ef46-133">application/json</span><span class="sxs-lookup"><span data-stu-id="2ef46-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ef46-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef46-134">Request body</span></span>
<span data-ttu-id="2ef46-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ef46-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ef46-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef46-136">Response</span></span>
<span data-ttu-id="2ef46-137">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileApp](../resources/intune-shared-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef46-137">If successful, this method returns a `200 OK` response code and [mobileApp](../resources/intune-shared-mobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef46-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ef46-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ef46-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef46-139">Request</span></span>
<span data-ttu-id="2ef46-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ef46-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="2ef46-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef46-141">Response</span></span>
<span data-ttu-id="2ef46-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ef46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






