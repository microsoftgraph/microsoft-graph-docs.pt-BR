---
title: Obter macOSMicrosoftEdgeApp
description: Leia as propriedades e as relações do objeto macOSMicrosoftEdgeApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a222dcd2e29c7c5d6db823bfbed24a5f7b2c879b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416309"
---
# <a name="get-macosmicrosoftedgeapp"></a><span data-ttu-id="3582e-103">Obter macOSMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="3582e-103">Get macOSMicrosoftEdgeApp</span></span>

<span data-ttu-id="3582e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3582e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3582e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3582e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3582e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3582e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3582e-107">Leia as propriedades e as relações do objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3582e-107">Read properties and relationships of the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3582e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3582e-108">Prerequisites</span></span>
<span data-ttu-id="3582e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3582e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3582e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3582e-111">Permission type</span></span>|<span data-ttu-id="3582e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3582e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3582e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3582e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3582e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3582e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3582e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3582e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3582e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3582e-116">Not supported.</span></span>|
|<span data-ttu-id="3582e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3582e-117">Application</span></span>|<span data-ttu-id="3582e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3582e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3582e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3582e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3582e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3582e-120">Optional query parameters</span></span>
<span data-ttu-id="3582e-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3582e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3582e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3582e-122">Request headers</span></span>
|<span data-ttu-id="3582e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3582e-123">Header</span></span>|<span data-ttu-id="3582e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3582e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3582e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3582e-125">Authorization</span></span>|<span data-ttu-id="3582e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3582e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3582e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3582e-127">Accept</span></span>|<span data-ttu-id="3582e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3582e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3582e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3582e-129">Request body</span></span>
<span data-ttu-id="3582e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3582e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3582e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3582e-131">Response</span></span>
<span data-ttu-id="3582e-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3582e-132">If successful, this method returns a `200 OK` response code and [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3582e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3582e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3582e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3582e-134">Request</span></span>
<span data-ttu-id="3582e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3582e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3582e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3582e-136">Response</span></span>
<span data-ttu-id="3582e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3582e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 985

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
    "id": "c964092a-092a-c964-2a09-64c92a0964c9",
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
    "channel": "beta"
  }
}
```



