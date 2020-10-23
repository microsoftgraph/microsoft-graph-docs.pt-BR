---
title: Atualizar managedDeviceMobileAppConfigurationAssignment
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8e3b202f49c4d54e61ff4501090b3a1909a202d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699440"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="f9ec6-103">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f9ec6-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="f9ec6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9ec6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9ec6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9ec6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ec6-107">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f9ec6-107">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9ec6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9ec6-108">Prerequisites</span></span>
<span data-ttu-id="f9ec6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ec6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9ec6-111">Permission type</span></span>|<span data-ttu-id="f9ec6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9ec6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9ec6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9ec6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9ec6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ec6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9ec6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9ec6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9ec6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-116">Not supported.</span></span>|
|<span data-ttu-id="f9ec6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9ec6-117">Application</span></span>|<span data-ttu-id="f9ec6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ec6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9ec6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ec6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f9ec6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ec6-120">Request headers</span></span>
|<span data-ttu-id="f9ec6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9ec6-121">Header</span></span>|<span data-ttu-id="f9ec6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9ec6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9ec6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9ec6-123">Authorization</span></span>|<span data-ttu-id="f9ec6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9ec6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9ec6-125">Accept</span></span>|<span data-ttu-id="f9ec6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9ec6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9ec6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ec6-127">Request body</span></span>
<span data-ttu-id="f9ec6-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f9ec6-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="f9ec6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f9ec6-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="f9ec6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9ec6-130">Property</span></span>|<span data-ttu-id="f9ec6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9ec6-131">Type</span></span>|<span data-ttu-id="f9ec6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9ec6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9ec6-133">id</span><span class="sxs-lookup"><span data-stu-id="f9ec6-133">id</span></span>|<span data-ttu-id="f9ec6-134">String</span><span class="sxs-lookup"><span data-stu-id="f9ec6-134">String</span></span>|<span data-ttu-id="f9ec6-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f9ec6-136">destino</span><span class="sxs-lookup"><span data-stu-id="f9ec6-136">target</span></span>|[<span data-ttu-id="f9ec6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f9ec6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f9ec6-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="f9ec6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ec6-139">Response</span></span>
<span data-ttu-id="f9ec6-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-140">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9ec6-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9ec6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9ec6-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ec6-142">Request</span></span>
<span data-ttu-id="f9ec6-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9ec6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ec6-144">Response</span></span>
<span data-ttu-id="f9ec6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9ec6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





