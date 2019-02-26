---
title: Acessar managedMobileLobApp
description: Leia as propriedades e as relações do objeto managedMobileLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1dd510ef171a4e03f6e37a401752569c550ec95
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146981"
---
# <a name="get-managedmobilelobapp"></a><span data-ttu-id="d6744-103">Acessar managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="d6744-103">Get managedMobileLobApp</span></span>

> <span data-ttu-id="d6744-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6744-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6744-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6744-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6744-106">Leia as propriedades e as relações do objeto [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d6744-106">Read properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6744-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6744-107">Prerequisites</span></span>
<span data-ttu-id="d6744-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d6744-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6744-110">Permission type</span></span>|<span data-ttu-id="d6744-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6744-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6744-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6744-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6744-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6744-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d6744-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6744-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6744-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6744-115">Not supported.</span></span>|
|<span data-ttu-id="d6744-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6744-116">Application</span></span>|<span data-ttu-id="d6744-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6744-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6744-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6744-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6744-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d6744-119">Optional query parameters</span></span>
<span data-ttu-id="d6744-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6744-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6744-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6744-121">Request headers</span></span>
|<span data-ttu-id="d6744-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6744-122">Header</span></span>|<span data-ttu-id="d6744-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d6744-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6744-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6744-124">Authorization</span></span>|<span data-ttu-id="d6744-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6744-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6744-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6744-126">Accept</span></span>|<span data-ttu-id="d6744-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d6744-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6744-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6744-128">Request body</span></span>
<span data-ttu-id="d6744-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6744-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6744-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6744-130">Response</span></span>
<span data-ttu-id="d6744-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6744-131">If successful, this method returns a `200 OK` response code and [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6744-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6744-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6744-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6744-133">Request</span></span>
<span data-ttu-id="d6744-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6744-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d6744-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6744-135">Response</span></span>
<span data-ttu-id="d6744-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6744-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1124

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileLobApp",
    "id": "cded7cc4-7cc4-cded-c47c-edcdc47cedcd",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4
  }
}
```




