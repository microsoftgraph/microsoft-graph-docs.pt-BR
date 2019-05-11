---
title: Obter intuneBrandingProfileAssignment
description: Leia as propriedades e as relações do objeto intuneBrandingProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e12a60dadccb275808891da3ac60b0066ebd82c4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898298"
---
# <a name="get-intunebrandingprofileassignment"></a><span data-ttu-id="2d9eb-103">Obter intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="2d9eb-103">Get intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="2d9eb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d9eb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d9eb-106">Leia as propriedades e as relações do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2d9eb-106">Read properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d9eb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d9eb-107">Prerequisites</span></span>
<span data-ttu-id="2d9eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d9eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d9eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d9eb-110">Permission type</span></span>|<span data-ttu-id="2d9eb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d9eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d9eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d9eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d9eb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d9eb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2d9eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d9eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d9eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-115">Not supported.</span></span>|
|<span data-ttu-id="2d9eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d9eb-116">Application</span></span>|<span data-ttu-id="2d9eb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d9eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d9eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d9eb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2d9eb-119">Optional query parameters</span></span>
<span data-ttu-id="2d9eb-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d9eb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d9eb-121">Request headers</span></span>
|<span data-ttu-id="2d9eb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d9eb-122">Header</span></span>|<span data-ttu-id="2d9eb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2d9eb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d9eb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d9eb-124">Authorization</span></span>|<span data-ttu-id="2d9eb-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d9eb-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d9eb-126">Accept</span></span>|<span data-ttu-id="2d9eb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2d9eb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d9eb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d9eb-128">Request body</span></span>
<span data-ttu-id="2d9eb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d9eb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d9eb-130">Response</span></span>
<span data-ttu-id="2d9eb-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d9eb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d9eb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d9eb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d9eb-133">Request</span></span>
<span data-ttu-id="2d9eb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="2d9eb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d9eb-135">Response</span></span>
<span data-ttu-id="2d9eb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d9eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": {
    "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
    "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




