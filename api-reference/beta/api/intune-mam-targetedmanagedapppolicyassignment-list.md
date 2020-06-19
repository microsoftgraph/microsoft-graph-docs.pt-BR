---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a07e57d5718b1fb9e53c612f9ea9e898c51f95ac
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791907"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="711bf-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="711bf-103">List targetedManagedAppPolicyAssignments</span></span>

<span data-ttu-id="711bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="711bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="711bf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="711bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="711bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="711bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="711bf-107">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="711bf-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="711bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="711bf-108">Prerequisites</span></span>
<span data-ttu-id="711bf-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="711bf-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="711bf-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="711bf-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="711bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="711bf-111">Permission type</span></span>|<span data-ttu-id="711bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="711bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="711bf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="711bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="711bf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="711bf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="711bf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="711bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="711bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="711bf-116">Not supported.</span></span>|
|<span data-ttu-id="711bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="711bf-117">Application</span></span>|<span data-ttu-id="711bf-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="711bf-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="711bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="711bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="711bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="711bf-120">Request headers</span></span>
|<span data-ttu-id="711bf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="711bf-121">Header</span></span>|<span data-ttu-id="711bf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="711bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="711bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="711bf-123">Authorization</span></span>|<span data-ttu-id="711bf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="711bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="711bf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="711bf-125">Accept</span></span>|<span data-ttu-id="711bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="711bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="711bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="711bf-127">Request body</span></span>
<span data-ttu-id="711bf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="711bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="711bf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="711bf-129">Response</span></span>
<span data-ttu-id="711bf-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="711bf-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="711bf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="711bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="711bf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="711bf-132">Request</span></span>
<span data-ttu-id="711bf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="711bf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="711bf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="711bf-134">Response</span></span>
<span data-ttu-id="711bf-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="711bf-135">Here is an example of the response.</span></span> <span data-ttu-id="711bf-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="711bf-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="711bf-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="711bf-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



