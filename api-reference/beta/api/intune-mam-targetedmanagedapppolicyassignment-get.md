---
title: Get targetedManagedAppPolicyAssignment
description: Ler propriedades e relações do objeto targetedManagedAppPolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8a4f3156369318db399bce01576547f4b0f283e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086862"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="e022c-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e022c-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="e022c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e022c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e022c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e022c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e022c-106">Ler propriedades e relações do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e022c-106">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e022c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e022c-107">Prerequisites</span></span>
<span data-ttu-id="e022c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e022c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e022c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e022c-110">Permission type</span></span>|<span data-ttu-id="e022c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e022c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e022c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e022c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e022c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e022c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e022c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e022c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e022c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e022c-115">Not supported.</span></span>|
|<span data-ttu-id="e022c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e022c-116">Application</span></span>|<span data-ttu-id="e022c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e022c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e022c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e022c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e022c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e022c-119">Optional query parameters</span></span>
<span data-ttu-id="e022c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e022c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e022c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e022c-121">Request headers</span></span>
|<span data-ttu-id="e022c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e022c-122">Header</span></span>|<span data-ttu-id="e022c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e022c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e022c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e022c-124">Authorization</span></span>|<span data-ttu-id="e022c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e022c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e022c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e022c-126">Accept</span></span>|<span data-ttu-id="e022c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e022c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e022c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e022c-128">Request body</span></span>
<span data-ttu-id="e022c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e022c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e022c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e022c-130">Response</span></span>
<span data-ttu-id="e022c-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e022c-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e022c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e022c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e022c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e022c-133">Request</span></span>
<span data-ttu-id="e022c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e022c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e022c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e022c-135">Response</span></span>
<span data-ttu-id="e022c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e022c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
    "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```






