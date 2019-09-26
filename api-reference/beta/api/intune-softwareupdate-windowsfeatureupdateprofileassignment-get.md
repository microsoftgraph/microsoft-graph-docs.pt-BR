---
title: Obter windowsFeatureUpdateProfileAssignment
description: Leia as propriedades e as relações do objeto windowsFeatureUpdateProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f17f845ac907f270c03c2bdcf4cf6bb1189a12c5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199498"
---
# <a name="get-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="87cff-103">Obter windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="87cff-103">Get windowsFeatureUpdateProfileAssignment</span></span>

> <span data-ttu-id="87cff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87cff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87cff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87cff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87cff-106">Leia as propriedades e as relações do objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="87cff-106">Read properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87cff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87cff-107">Prerequisites</span></span>
<span data-ttu-id="87cff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87cff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87cff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87cff-110">Permission type</span></span>|<span data-ttu-id="87cff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87cff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87cff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87cff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87cff-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87cff-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87cff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87cff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87cff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87cff-115">Not supported.</span></span>|
|<span data-ttu-id="87cff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87cff-116">Application</span></span>|<span data-ttu-id="87cff-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87cff-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87cff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87cff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87cff-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87cff-119">Optional query parameters</span></span>
<span data-ttu-id="87cff-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87cff-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87cff-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87cff-121">Request headers</span></span>
|<span data-ttu-id="87cff-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87cff-122">Header</span></span>|<span data-ttu-id="87cff-123">Valor</span><span class="sxs-lookup"><span data-stu-id="87cff-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87cff-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="87cff-124">Authorization</span></span>|<span data-ttu-id="87cff-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87cff-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87cff-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87cff-126">Accept</span></span>|<span data-ttu-id="87cff-127">application/json</span><span class="sxs-lookup"><span data-stu-id="87cff-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87cff-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87cff-128">Request body</span></span>
<span data-ttu-id="87cff-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87cff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87cff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="87cff-130">Response</span></span>
<span data-ttu-id="87cff-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87cff-131">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87cff-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87cff-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="87cff-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87cff-133">Request</span></span>
<span data-ttu-id="87cff-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87cff-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="87cff-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="87cff-135">Response</span></span>
<span data-ttu-id="87cff-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87cff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
    "id": "567a744f-744f-567a-4f74-7a564f747a56",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




