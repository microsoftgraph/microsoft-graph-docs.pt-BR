---
title: Obter mobileContainedApp
description: Leia as propriedades e as relações do objeto mobileContainedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ee816affa0cfbb89558b997cf273b829ef1d4fc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934795"
---
# <a name="get-mobilecontainedapp"></a><span data-ttu-id="24991-103">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="24991-103">Get mobileContainedApp</span></span>

> <span data-ttu-id="24991-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24991-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24991-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24991-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24991-106">Leia as propriedades e as relações do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="24991-106">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24991-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24991-107">Prerequisites</span></span>
<span data-ttu-id="24991-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24991-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24991-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24991-110">Permission type</span></span>|<span data-ttu-id="24991-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24991-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24991-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24991-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24991-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="24991-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="24991-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24991-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24991-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24991-115">Not supported.</span></span>|
|<span data-ttu-id="24991-116">Application</span><span class="sxs-lookup"><span data-stu-id="24991-116">Application</span></span>|<span data-ttu-id="24991-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="24991-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24991-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24991-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24991-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24991-119">Optional query parameters</span></span>
<span data-ttu-id="24991-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24991-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24991-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24991-121">Request headers</span></span>
|<span data-ttu-id="24991-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24991-122">Header</span></span>|<span data-ttu-id="24991-123">Valor</span><span class="sxs-lookup"><span data-stu-id="24991-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24991-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="24991-124">Authorization</span></span>|<span data-ttu-id="24991-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24991-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24991-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24991-126">Accept</span></span>|<span data-ttu-id="24991-127">application/json</span><span class="sxs-lookup"><span data-stu-id="24991-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24991-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24991-128">Request body</span></span>
<span data-ttu-id="24991-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24991-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24991-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="24991-130">Response</span></span>
<span data-ttu-id="24991-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24991-131">If successful, this method returns a `200 OK` response code and [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24991-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24991-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="24991-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24991-133">Request</span></span>
<span data-ttu-id="24991-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24991-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="24991-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="24991-135">Response</span></span>
<span data-ttu-id="24991-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24991-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





