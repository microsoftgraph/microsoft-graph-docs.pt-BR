---
title: Obter windowsFeatureUpdateProfileAssignment
description: Leia as propriedades e as relações do objeto windowsFeatureUpdateProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c776a6a3988b3e920a49a2c46ab29a1d3b841312
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536795"
---
# <a name="get-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="ae67b-103">Obter windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="ae67b-103">Get windowsFeatureUpdateProfileAssignment</span></span>

> <span data-ttu-id="ae67b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae67b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae67b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae67b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae67b-106">Leia as propriedades e as relações do objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ae67b-106">Read properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae67b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae67b-107">Prerequisites</span></span>
<span data-ttu-id="ae67b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae67b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae67b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae67b-110">Permission type</span></span>|<span data-ttu-id="ae67b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae67b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae67b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae67b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae67b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae67b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ae67b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae67b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae67b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae67b-115">Not supported.</span></span>|
|<span data-ttu-id="ae67b-116">Application</span><span class="sxs-lookup"><span data-stu-id="ae67b-116">Application</span></span>|<span data-ttu-id="ae67b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae67b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae67b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae67b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae67b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae67b-119">Optional query parameters</span></span>
<span data-ttu-id="ae67b-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae67b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae67b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae67b-121">Request headers</span></span>
|<span data-ttu-id="ae67b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae67b-122">Header</span></span>|<span data-ttu-id="ae67b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ae67b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae67b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae67b-124">Authorization</span></span>|<span data-ttu-id="ae67b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae67b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae67b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae67b-126">Accept</span></span>|<span data-ttu-id="ae67b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ae67b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae67b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae67b-128">Request body</span></span>
<span data-ttu-id="ae67b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae67b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae67b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae67b-130">Response</span></span>
<span data-ttu-id="ae67b-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae67b-131">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae67b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae67b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae67b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae67b-133">Request</span></span>
<span data-ttu-id="ae67b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae67b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ae67b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae67b-135">Response</span></span>
<span data-ttu-id="ae67b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae67b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






