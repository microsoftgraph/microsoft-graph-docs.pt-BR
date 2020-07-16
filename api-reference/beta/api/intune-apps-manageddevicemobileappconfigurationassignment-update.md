---
title: Atualizar managedDeviceMobileAppConfigurationAssignment
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91d2de2e43a3426d9d2ff9438f23945b277f4f72
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793343"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="d8790-103">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d8790-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="d8790-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8790-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8790-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8790-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8790-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8790-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8790-107">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8790-107">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8790-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8790-108">Prerequisites</span></span>
<span data-ttu-id="d8790-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8790-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8790-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8790-111">Permission type</span></span>|<span data-ttu-id="d8790-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8790-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8790-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8790-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8790-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8790-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8790-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8790-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8790-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8790-116">Not supported.</span></span>|
|<span data-ttu-id="d8790-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8790-117">Application</span></span>|<span data-ttu-id="d8790-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8790-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8790-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8790-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d8790-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8790-120">Request headers</span></span>
|<span data-ttu-id="d8790-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8790-121">Header</span></span>|<span data-ttu-id="d8790-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8790-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8790-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8790-123">Authorization</span></span>|<span data-ttu-id="d8790-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8790-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8790-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8790-125">Accept</span></span>|<span data-ttu-id="d8790-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8790-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8790-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8790-127">Request body</span></span>
<span data-ttu-id="d8790-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8790-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="d8790-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8790-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="d8790-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8790-130">Property</span></span>|<span data-ttu-id="d8790-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8790-131">Type</span></span>|<span data-ttu-id="d8790-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8790-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8790-133">id</span><span class="sxs-lookup"><span data-stu-id="d8790-133">id</span></span>|<span data-ttu-id="d8790-134">String</span><span class="sxs-lookup"><span data-stu-id="d8790-134">String</span></span>|<span data-ttu-id="d8790-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8790-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d8790-136">destino</span><span class="sxs-lookup"><span data-stu-id="d8790-136">target</span></span>|[<span data-ttu-id="d8790-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d8790-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d8790-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="d8790-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d8790-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8790-139">Response</span></span>
<span data-ttu-id="d8790-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8790-140">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8790-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8790-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8790-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8790-142">Request</span></span>
<span data-ttu-id="d8790-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8790-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
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

### <a name="response"></a><span data-ttu-id="d8790-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8790-144">Response</span></span>
<span data-ttu-id="d8790-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8790-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



