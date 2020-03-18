---
title: Obter intuneBrandingProfileAssignment
description: Leia as propriedades e as relações do objeto intuneBrandingProfileAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10801311e5e4f1a3ded5c6c4c0eade8dffa423cf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799685"
---
# <a name="get-intunebrandingprofileassignment"></a><span data-ttu-id="e99dd-103">Obter intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="e99dd-103">Get intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="e99dd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e99dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e99dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e99dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e99dd-106">Leia as propriedades e as relações do objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e99dd-106">Read properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e99dd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e99dd-107">Prerequisites</span></span>
<span data-ttu-id="e99dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e99dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e99dd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e99dd-110">Permission type</span></span>|<span data-ttu-id="e99dd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e99dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e99dd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e99dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e99dd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e99dd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e99dd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e99dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e99dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e99dd-115">Not supported.</span></span>|
|<span data-ttu-id="e99dd-116">Application</span><span class="sxs-lookup"><span data-stu-id="e99dd-116">Application</span></span>|<span data-ttu-id="e99dd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e99dd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e99dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e99dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e99dd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e99dd-119">Optional query parameters</span></span>
<span data-ttu-id="e99dd-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e99dd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e99dd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e99dd-121">Request headers</span></span>
|<span data-ttu-id="e99dd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e99dd-122">Header</span></span>|<span data-ttu-id="e99dd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e99dd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e99dd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e99dd-124">Authorization</span></span>|<span data-ttu-id="e99dd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e99dd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e99dd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e99dd-126">Accept</span></span>|<span data-ttu-id="e99dd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e99dd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e99dd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e99dd-128">Request body</span></span>
<span data-ttu-id="e99dd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e99dd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e99dd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e99dd-130">Response</span></span>
<span data-ttu-id="e99dd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e99dd-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e99dd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e99dd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e99dd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e99dd-133">Request</span></span>
<span data-ttu-id="e99dd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e99dd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e99dd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e99dd-135">Response</span></span>
<span data-ttu-id="e99dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e99dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




