---
title: Atualizar managedDeviceMobileAppConfigurationAssignment
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: a9c1c7b1f0af2ec49080d6b6e225d3923b7f37b5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301432"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="6e4cd-103">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6e4cd-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="6e4cd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e4cd-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6e4cd-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e4cd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e4cd-106">Prerequisites</span></span>
<span data-ttu-id="6e4cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e4cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e4cd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e4cd-109">Permission type</span></span>|<span data-ttu-id="6e4cd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e4cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e4cd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e4cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e4cd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e4cd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6e4cd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e4cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e4cd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-114">Not supported.</span></span>|
|<span data-ttu-id="6e4cd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e4cd-115">Application</span></span>|<span data-ttu-id="6e4cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e4cd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e4cd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6e4cd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e4cd-118">Request headers</span></span>
|<span data-ttu-id="6e4cd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e4cd-119">Header</span></span>|<span data-ttu-id="6e4cd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6e4cd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e4cd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e4cd-121">Authorization</span></span>|<span data-ttu-id="6e4cd-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e4cd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6e4cd-123">Accept</span></span>|<span data-ttu-id="6e4cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6e4cd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e4cd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e4cd-125">Request body</span></span>
<span data-ttu-id="6e4cd-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6e4cd-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="6e4cd-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6e4cd-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="6e4cd-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e4cd-128">Property</span></span>|<span data-ttu-id="6e4cd-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e4cd-129">Type</span></span>|<span data-ttu-id="6e4cd-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e4cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e4cd-131">id</span><span class="sxs-lookup"><span data-stu-id="6e4cd-131">id</span></span>|<span data-ttu-id="6e4cd-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e4cd-132">String</span></span>|<span data-ttu-id="6e4cd-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6e4cd-134">destino</span><span class="sxs-lookup"><span data-stu-id="6e4cd-134">target</span></span>|[<span data-ttu-id="6e4cd-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6e4cd-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6e4cd-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="6e4cd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e4cd-137">Response</span></span>
<span data-ttu-id="6e4cd-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e4cd-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e4cd-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e4cd-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e4cd-140">Request</span></span>
<span data-ttu-id="6e4cd-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e4cd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e4cd-142">Response</span></span>
<span data-ttu-id="6e4cd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e4cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



