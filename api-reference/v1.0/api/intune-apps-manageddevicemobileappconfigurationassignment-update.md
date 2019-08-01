---
title: Atualizar managedDeviceMobileAppConfigurationAssignment
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5dfbcdc131dd02f062252974a7ef4b3baff07b1f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014036"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="7fe74-103">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7fe74-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="7fe74-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7fe74-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fe74-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7fe74-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fe74-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7fe74-106">Prerequisites</span></span>
<span data-ttu-id="7fe74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe74-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fe74-109">Permission type</span></span>|<span data-ttu-id="7fe74-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7fe74-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fe74-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fe74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7fe74-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe74-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7fe74-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fe74-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fe74-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe74-114">Not supported.</span></span>|
|<span data-ttu-id="7fe74-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fe74-115">Application</span></span>|<span data-ttu-id="7fe74-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe74-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe74-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe74-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7fe74-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe74-118">Request headers</span></span>
|<span data-ttu-id="7fe74-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fe74-119">Header</span></span>|<span data-ttu-id="7fe74-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7fe74-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fe74-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fe74-121">Authorization</span></span>|<span data-ttu-id="7fe74-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fe74-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fe74-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7fe74-123">Accept</span></span>|<span data-ttu-id="7fe74-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7fe74-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe74-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe74-125">Request body</span></span>
<span data-ttu-id="7fe74-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7fe74-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="7fe74-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7fe74-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="7fe74-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fe74-128">Property</span></span>|<span data-ttu-id="7fe74-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fe74-129">Type</span></span>|<span data-ttu-id="7fe74-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fe74-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fe74-131">id</span><span class="sxs-lookup"><span data-stu-id="7fe74-131">id</span></span>|<span data-ttu-id="7fe74-132">String</span><span class="sxs-lookup"><span data-stu-id="7fe74-132">String</span></span>|<span data-ttu-id="7fe74-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="7fe74-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7fe74-134">destino</span><span class="sxs-lookup"><span data-stu-id="7fe74-134">target</span></span>|[<span data-ttu-id="7fe74-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7fe74-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7fe74-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="7fe74-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="7fe74-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe74-137">Response</span></span>
<span data-ttu-id="7fe74-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe74-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe74-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fe74-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fe74-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe74-140">Request</span></span>
<span data-ttu-id="7fe74-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe74-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7fe74-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe74-142">Response</span></span>
<span data-ttu-id="7fe74-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



