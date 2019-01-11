---
title: Atualizar managedDeviceMobileAppConfigurationAssignment
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 58d28cb3e80f127f164e65861a15c230ef2d45fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864229"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="5ccb4-103">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5ccb4-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="5ccb4-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ccb4-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ccb4-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ccb4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ccb4-106">Prerequisites</span></span>
<span data-ttu-id="5ccb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ccb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ccb4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ccb4-109">Permission type</span></span>|<span data-ttu-id="5ccb4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ccb4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ccb4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ccb4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ccb4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ccb4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5ccb4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ccb4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ccb4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-114">Not supported.</span></span>|
|<span data-ttu-id="5ccb4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ccb4-115">Application</span></span>|<span data-ttu-id="5ccb4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ccb4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ccb4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5ccb4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccb4-118">Request headers</span></span>
|<span data-ttu-id="5ccb4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ccb4-119">Header</span></span>|<span data-ttu-id="5ccb4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5ccb4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ccb4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ccb4-121">Authorization</span></span>|<span data-ttu-id="5ccb4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ccb4-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ccb4-123">Accept</span></span>|<span data-ttu-id="5ccb4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5ccb4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ccb4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccb4-125">Request body</span></span>
<span data-ttu-id="5ccb4-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ccb4-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="5ccb4-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ccb4-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="5ccb4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ccb4-128">Property</span></span>|<span data-ttu-id="5ccb4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ccb4-129">Type</span></span>|<span data-ttu-id="5ccb4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ccb4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ccb4-131">id</span><span class="sxs-lookup"><span data-stu-id="5ccb4-131">id</span></span>|<span data-ttu-id="5ccb4-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ccb4-132">String</span></span>|<span data-ttu-id="5ccb4-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5ccb4-134">destino</span><span class="sxs-lookup"><span data-stu-id="5ccb4-134">target</span></span>|[<span data-ttu-id="5ccb4-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5ccb4-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5ccb4-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5ccb4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ccb4-137">Response</span></span>
<span data-ttu-id="5ccb4-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ccb4-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ccb4-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ccb4-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ccb4-140">Request</span></span>
<span data-ttu-id="5ccb4-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ccb4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ccb4-142">Response</span></span>
<span data-ttu-id="5ccb4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ccb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



