---
title: Atualizar managedDeviceMobileAppConfigurationAssignment
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dccf48cfefb0e5a9f09fd51e998a1172280f72d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982564"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="8c8d6-103">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8c8d6-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="8c8d6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c8d6-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c8d6-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c8d6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c8d6-106">Prerequisites</span></span>
<span data-ttu-id="8c8d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c8d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c8d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c8d6-109">Permission type</span></span>|<span data-ttu-id="8c8d6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c8d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c8d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c8d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c8d6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c8d6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c8d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c8d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c8d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-114">Not supported.</span></span>|
|<span data-ttu-id="8c8d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c8d6-115">Application</span></span>|<span data-ttu-id="8c8d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c8d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c8d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8c8d6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8d6-118">Request headers</span></span>
|<span data-ttu-id="8c8d6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c8d6-119">Header</span></span>|<span data-ttu-id="8c8d6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8c8d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c8d6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c8d6-121">Authorization</span></span>|<span data-ttu-id="8c8d6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c8d6-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c8d6-123">Accept</span></span>|<span data-ttu-id="8c8d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c8d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c8d6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8d6-125">Request body</span></span>
<span data-ttu-id="8c8d6-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c8d6-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="8c8d6-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c8d6-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="8c8d6-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c8d6-128">Property</span></span>|<span data-ttu-id="8c8d6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c8d6-129">Type</span></span>|<span data-ttu-id="8c8d6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c8d6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c8d6-131">id</span><span class="sxs-lookup"><span data-stu-id="8c8d6-131">id</span></span>|<span data-ttu-id="8c8d6-132">String</span><span class="sxs-lookup"><span data-stu-id="8c8d6-132">String</span></span>|<span data-ttu-id="8c8d6-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="8c8d6-134">destino</span><span class="sxs-lookup"><span data-stu-id="8c8d6-134">target</span></span>|[<span data-ttu-id="8c8d6-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8c8d6-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8c8d6-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="8c8d6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c8d6-137">Response</span></span>
<span data-ttu-id="8c8d6-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c8d6-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c8d6-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c8d6-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c8d6-140">Request</span></span>
<span data-ttu-id="8c8d6-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8c8d6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c8d6-142">Response</span></span>
<span data-ttu-id="8c8d6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c8d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



