---
title: Listar targetedManagedAppPolicyAssignments
description: Listar propriedades e relações de objetos de targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 415808e1a262f869aeb013a467e385e212920ac7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694421"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="e4f61-103">Listar targetedManagedAppPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="e4f61-103">List targetedManagedAppPolicyAssignments</span></span>

<span data-ttu-id="e4f61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4f61-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4f61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4f61-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4f61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4f61-107">Listar propriedades e relações de objetos de [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e4f61-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4f61-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4f61-108">Prerequisites</span></span>
<span data-ttu-id="e4f61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4f61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4f61-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4f61-111">Permission type</span></span>|<span data-ttu-id="e4f61-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4f61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4f61-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4f61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4f61-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4f61-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e4f61-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4f61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4f61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4f61-116">Not supported.</span></span>|
|<span data-ttu-id="e4f61-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4f61-117">Application</span></span>|<span data-ttu-id="e4f61-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4f61-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4f61-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4f61-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e4f61-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f61-120">Request headers</span></span>
|<span data-ttu-id="e4f61-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4f61-121">Header</span></span>|<span data-ttu-id="e4f61-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e4f61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4f61-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4f61-123">Authorization</span></span>|<span data-ttu-id="e4f61-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4f61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4f61-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4f61-125">Accept</span></span>|<span data-ttu-id="e4f61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4f61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4f61-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f61-127">Request body</span></span>
<span data-ttu-id="e4f61-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4f61-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4f61-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4f61-129">Response</span></span>
<span data-ttu-id="e4f61-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4f61-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4f61-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4f61-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4f61-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f61-132">Request</span></span>
<span data-ttu-id="e4f61-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4f61-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="e4f61-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4f61-134">Response</span></span>
<span data-ttu-id="e4f61-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4f61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





