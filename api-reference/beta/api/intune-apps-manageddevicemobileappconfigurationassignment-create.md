---
title: Criar managedDeviceMobileAppConfigurationAssignment
description: Criar um novo objeto managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6514f3f6cc6e1c230878773dd941e145cef9bfa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014949"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="d9294-103">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d9294-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="d9294-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9294-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9294-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9294-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9294-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9294-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9294-107">Criar um novo objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d9294-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9294-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9294-108">Prerequisites</span></span>
<span data-ttu-id="d9294-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9294-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9294-111">Permission type</span></span>|<span data-ttu-id="d9294-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9294-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9294-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9294-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9294-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9294-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9294-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9294-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9294-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9294-116">Not supported.</span></span>|
|<span data-ttu-id="d9294-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9294-117">Application</span></span>|<span data-ttu-id="d9294-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9294-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9294-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9294-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d9294-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9294-120">Request headers</span></span>
|<span data-ttu-id="d9294-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9294-121">Header</span></span>|<span data-ttu-id="d9294-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d9294-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9294-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9294-123">Authorization</span></span>|<span data-ttu-id="d9294-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9294-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9294-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9294-125">Accept</span></span>|<span data-ttu-id="d9294-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9294-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9294-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9294-127">Request body</span></span>
<span data-ttu-id="d9294-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="d9294-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="d9294-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="d9294-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="d9294-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9294-130">Property</span></span>|<span data-ttu-id="d9294-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9294-131">Type</span></span>|<span data-ttu-id="d9294-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9294-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9294-133">id</span><span class="sxs-lookup"><span data-stu-id="d9294-133">id</span></span>|<span data-ttu-id="d9294-134">String</span><span class="sxs-lookup"><span data-stu-id="d9294-134">String</span></span>|<span data-ttu-id="d9294-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9294-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d9294-136">destino</span><span class="sxs-lookup"><span data-stu-id="d9294-136">target</span></span>|[<span data-ttu-id="d9294-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9294-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d9294-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="d9294-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d9294-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9294-139">Response</span></span>
<span data-ttu-id="d9294-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9294-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9294-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9294-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9294-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9294-142">Request</span></span>
<span data-ttu-id="d9294-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9294-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="d9294-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9294-144">Response</span></span>
<span data-ttu-id="d9294-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9294-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 395

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```






