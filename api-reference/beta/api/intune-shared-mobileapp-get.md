---
title: Acessar mobileApp
description: Leia as propriedades e as relações do objeto mobileApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2fe080267c2f2a231282e6ba8f35e324b887fa7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448649"
---
# <a name="get-mobileapp"></a><span data-ttu-id="04336-103">Acessar mobileApp</span><span class="sxs-lookup"><span data-stu-id="04336-103">Get mobileApp</span></span>

<span data-ttu-id="04336-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04336-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04336-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04336-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04336-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04336-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04336-107">Leia as propriedades e as relações do objeto [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04336-107">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04336-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04336-108">Prerequisites</span></span>
<span data-ttu-id="04336-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04336-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04336-111">Permission type</span></span>|<span data-ttu-id="04336-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04336-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04336-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04336-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="04336-114">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="04336-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="04336-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="04336-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="04336-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="04336-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="04336-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="04336-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="04336-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04336-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04336-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04336-119">Not supported.</span></span>|
|<span data-ttu-id="04336-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04336-120">Application</span></span>||
| <span data-ttu-id="04336-121">&nbsp; &nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="04336-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="04336-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="04336-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="04336-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="04336-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="04336-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="04336-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04336-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04336-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04336-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04336-126">Optional query parameters</span></span>
<span data-ttu-id="04336-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04336-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04336-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04336-128">Request headers</span></span>
|<span data-ttu-id="04336-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04336-129">Header</span></span>|<span data-ttu-id="04336-130">Valor</span><span class="sxs-lookup"><span data-stu-id="04336-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04336-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="04336-131">Authorization</span></span>|<span data-ttu-id="04336-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04336-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04336-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04336-133">Accept</span></span>|<span data-ttu-id="04336-134">application/json</span><span class="sxs-lookup"><span data-stu-id="04336-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04336-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04336-135">Request body</span></span>
<span data-ttu-id="04336-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04336-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04336-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="04336-137">Response</span></span>
<span data-ttu-id="04336-138">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileApp](../resources/intune-shared-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04336-138">If successful, this method returns a `200 OK` response code and [mobileApp](../resources/intune-shared-mobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04336-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04336-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="04336-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04336-140">Request</span></span>
<span data-ttu-id="04336-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04336-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="04336-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="04336-142">Response</span></span>
<span data-ttu-id="04336-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04336-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






