---
title: Obter appleEnrollmentProfileAssignment
description: Leia as propriedades e as relações do objeto appleEnrollmentProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d515224281c608760b347fbcdcb255a435efae14
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087331"
---
# <a name="get-appleenrollmentprofileassignment"></a><span data-ttu-id="e2ac4-103">Obter appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="e2ac4-103">Get appleEnrollmentProfileAssignment</span></span>

> <span data-ttu-id="e2ac4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2ac4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2ac4-106">Leia as propriedades e as relações do objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e2ac4-106">Read properties and relationships of the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2ac4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2ac4-107">Prerequisites</span></span>
<span data-ttu-id="e2ac4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2ac4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2ac4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2ac4-110">Permission type</span></span>|<span data-ttu-id="e2ac4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2ac4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2ac4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2ac4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2ac4-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2ac4-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e2ac4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2ac4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2ac4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-115">Not supported.</span></span>|
|<span data-ttu-id="e2ac4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2ac4-116">Application</span></span>|<span data-ttu-id="e2ac4-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2ac4-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2ac4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2ac4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2ac4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e2ac4-119">Optional query parameters</span></span>
<span data-ttu-id="e2ac4-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2ac4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2ac4-121">Request headers</span></span>
|<span data-ttu-id="e2ac4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2ac4-122">Header</span></span>|<span data-ttu-id="e2ac4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e2ac4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2ac4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2ac4-124">Authorization</span></span>|<span data-ttu-id="e2ac4-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2ac4-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2ac4-126">Accept</span></span>|<span data-ttu-id="e2ac4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e2ac4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2ac4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2ac4-128">Request body</span></span>
<span data-ttu-id="e2ac4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2ac4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2ac4-130">Response</span></span>
<span data-ttu-id="e2ac4-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-131">If successful, this method returns a `200 OK` response code and [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2ac4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2ac4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2ac4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2ac4-133">Request</span></span>
<span data-ttu-id="e2ac4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e2ac4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2ac4-135">Response</span></span>
<span data-ttu-id="e2ac4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2ac4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
    "id": "5b603771-3771-5b60-7137-605b7137605b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```






