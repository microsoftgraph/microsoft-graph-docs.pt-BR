---
title: Obter mobileContainedApp
description: Leia as propriedades e as relações do objeto mobileContainedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59f6f6ac4d685a0df9989a308d9b64de9d501dba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336436"
---
# <a name="get-mobilecontainedapp"></a><span data-ttu-id="574be-103">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="574be-103">Get mobileContainedApp</span></span>

> <span data-ttu-id="574be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="574be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="574be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="574be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="574be-106">Leia as propriedades e as relações do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="574be-106">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="574be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="574be-107">Prerequisites</span></span>
<span data-ttu-id="574be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="574be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="574be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="574be-110">Permission type</span></span>|<span data-ttu-id="574be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="574be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="574be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="574be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="574be-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="574be-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="574be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="574be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="574be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="574be-115">Not supported.</span></span>|
|<span data-ttu-id="574be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="574be-116">Application</span></span>|<span data-ttu-id="574be-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="574be-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="574be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="574be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="574be-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="574be-119">Optional query parameters</span></span>
<span data-ttu-id="574be-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="574be-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="574be-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="574be-121">Request headers</span></span>
|<span data-ttu-id="574be-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="574be-122">Header</span></span>|<span data-ttu-id="574be-123">Valor</span><span class="sxs-lookup"><span data-stu-id="574be-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="574be-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="574be-124">Authorization</span></span>|<span data-ttu-id="574be-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="574be-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="574be-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="574be-126">Accept</span></span>|<span data-ttu-id="574be-127">application/json</span><span class="sxs-lookup"><span data-stu-id="574be-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="574be-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="574be-128">Request body</span></span>
<span data-ttu-id="574be-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="574be-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="574be-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="574be-130">Response</span></span>
<span data-ttu-id="574be-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="574be-131">If successful, this method returns a `200 OK` response code and [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="574be-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="574be-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="574be-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="574be-133">Request</span></span>
<span data-ttu-id="574be-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="574be-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="574be-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="574be-135">Response</span></span>
<span data-ttu-id="574be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="574be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileContainedApp",
    "id": "3c02d875-d875-3c02-75d8-023c75d8023c"
  }
}
```






