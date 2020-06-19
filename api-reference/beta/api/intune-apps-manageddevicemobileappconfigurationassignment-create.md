---
title: Criar managedDeviceMobileAppConfigurationAssignment
description: Criar um novo objeto managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9bd6d4ab40942e588be370724b1d0cc8f80a529
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793364"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="61522-103">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="61522-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="61522-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61522-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61522-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61522-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61522-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61522-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61522-107">Criar um novo objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="61522-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61522-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61522-108">Prerequisites</span></span>
<span data-ttu-id="61522-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="61522-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="61522-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61522-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61522-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61522-111">Permission type</span></span>|<span data-ttu-id="61522-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61522-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61522-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61522-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61522-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61522-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61522-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61522-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61522-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61522-116">Not supported.</span></span>|
|<span data-ttu-id="61522-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61522-117">Application</span></span>|<span data-ttu-id="61522-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61522-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61522-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61522-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="61522-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61522-120">Request headers</span></span>
|<span data-ttu-id="61522-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61522-121">Header</span></span>|<span data-ttu-id="61522-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61522-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61522-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61522-123">Authorization</span></span>|<span data-ttu-id="61522-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61522-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61522-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61522-125">Accept</span></span>|<span data-ttu-id="61522-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61522-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61522-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61522-127">Request body</span></span>
<span data-ttu-id="61522-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="61522-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="61522-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="61522-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="61522-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61522-130">Property</span></span>|<span data-ttu-id="61522-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="61522-131">Type</span></span>|<span data-ttu-id="61522-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61522-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61522-133">id</span><span class="sxs-lookup"><span data-stu-id="61522-133">id</span></span>|<span data-ttu-id="61522-134">String</span><span class="sxs-lookup"><span data-stu-id="61522-134">String</span></span>|<span data-ttu-id="61522-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="61522-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="61522-136">destino</span><span class="sxs-lookup"><span data-stu-id="61522-136">target</span></span>|[<span data-ttu-id="61522-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="61522-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="61522-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="61522-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="61522-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="61522-139">Response</span></span>
<span data-ttu-id="61522-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61522-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61522-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61522-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="61522-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61522-142">Request</span></span>
<span data-ttu-id="61522-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61522-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="61522-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="61522-144">Response</span></span>
<span data-ttu-id="61522-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="61522-145">Here is an example of the response.</span></span> <span data-ttu-id="61522-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="61522-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="61522-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="61522-147">All of the properties will be returned from an actual call.</span></span>
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



