---
title: Atualizar targetedManagedAppPolicyAssignment
description: Atualizar as propriedades de um objeto targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32e03d719a631e1237eafac4404f9a9607dde188
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988053"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="86c10-103">Atualizar targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="86c10-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="86c10-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86c10-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86c10-105">Atualizar as propriedades de um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="86c10-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86c10-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86c10-106">Prerequisites</span></span>
<span data-ttu-id="86c10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86c10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86c10-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86c10-109">Permission type</span></span>|<span data-ttu-id="86c10-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86c10-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86c10-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86c10-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86c10-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c10-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86c10-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86c10-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86c10-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86c10-114">Not supported.</span></span>|
|<span data-ttu-id="86c10-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86c10-115">Application</span></span>|<span data-ttu-id="86c10-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86c10-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86c10-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86c10-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="86c10-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86c10-118">Request headers</span></span>
|<span data-ttu-id="86c10-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86c10-119">Header</span></span>|<span data-ttu-id="86c10-120">Valor</span><span class="sxs-lookup"><span data-stu-id="86c10-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86c10-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="86c10-121">Authorization</span></span>|<span data-ttu-id="86c10-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86c10-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86c10-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86c10-123">Accept</span></span>|<span data-ttu-id="86c10-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86c10-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86c10-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86c10-125">Request body</span></span>
<span data-ttu-id="86c10-126">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="86c10-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="86c10-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="86c10-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="86c10-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86c10-128">Property</span></span>|<span data-ttu-id="86c10-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="86c10-129">Type</span></span>|<span data-ttu-id="86c10-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="86c10-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86c10-131">id</span><span class="sxs-lookup"><span data-stu-id="86c10-131">id</span></span>|<span data-ttu-id="86c10-132">String</span><span class="sxs-lookup"><span data-stu-id="86c10-132">String</span></span>|<span data-ttu-id="86c10-133">Id</span><span class="sxs-lookup"><span data-stu-id="86c10-133">Id</span></span>|
|<span data-ttu-id="86c10-134">destino</span><span class="sxs-lookup"><span data-stu-id="86c10-134">target</span></span>|[<span data-ttu-id="86c10-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="86c10-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="86c10-136">Identificador de implantação de um grupo ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="86c10-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="86c10-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c10-137">Response</span></span>
<span data-ttu-id="86c10-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86c10-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c10-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86c10-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="86c10-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86c10-140">Request</span></span>
<span data-ttu-id="86c10-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86c10-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="86c10-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c10-142">Response</span></span>
<span data-ttu-id="86c10-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86c10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



