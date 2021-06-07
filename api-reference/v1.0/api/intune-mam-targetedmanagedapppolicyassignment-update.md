---
title: Atualizar targetedManagedAppPolicyAssignment
description: Atualizar as propriedades de um objeto targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 824d406f33003736c1c0304b6a5af3b106d4ccd6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752585"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="5ae88-103">Atualizar targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5ae88-103">Update targetedManagedAppPolicyAssignment</span></span>

<span data-ttu-id="5ae88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ae88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ae88-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ae88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ae88-106">Atualizar as propriedades de um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ae88-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ae88-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ae88-107">Prerequisites</span></span>
<span data-ttu-id="5ae88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ae88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ae88-110">Permission type</span></span>|<span data-ttu-id="5ae88-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ae88-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ae88-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ae88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ae88-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae88-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5ae88-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ae88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ae88-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ae88-115">Not supported.</span></span>|
|<span data-ttu-id="5ae88-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ae88-116">Application</span></span>|<span data-ttu-id="5ae88-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae88-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ae88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ae88-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5ae88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ae88-119">Request headers</span></span>
|<span data-ttu-id="5ae88-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ae88-120">Header</span></span>|<span data-ttu-id="5ae88-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ae88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ae88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ae88-122">Authorization</span></span>|<span data-ttu-id="5ae88-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ae88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ae88-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ae88-124">Accept</span></span>|<span data-ttu-id="5ae88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ae88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ae88-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ae88-126">Request body</span></span>
<span data-ttu-id="5ae88-127">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ae88-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="5ae88-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ae88-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="5ae88-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ae88-129">Property</span></span>|<span data-ttu-id="5ae88-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ae88-130">Type</span></span>|<span data-ttu-id="5ae88-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ae88-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ae88-132">id</span><span class="sxs-lookup"><span data-stu-id="5ae88-132">id</span></span>|<span data-ttu-id="5ae88-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ae88-133">String</span></span>|<span data-ttu-id="5ae88-134">Id</span><span class="sxs-lookup"><span data-stu-id="5ae88-134">Id</span></span>|
|<span data-ttu-id="5ae88-135">destino</span><span class="sxs-lookup"><span data-stu-id="5ae88-135">target</span></span>|[<span data-ttu-id="5ae88-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5ae88-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5ae88-137">Identificador de implantação para um grupo ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ae88-137">Identifier for deployment to a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="5ae88-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ae88-138">Response</span></span>
<span data-ttu-id="5ae88-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ae88-139">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ae88-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ae88-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ae88-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ae88-141">Request</span></span>
<span data-ttu-id="5ae88-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ae88-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 226

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="5ae88-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ae88-143">Response</span></span>
<span data-ttu-id="5ae88-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ae88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```




