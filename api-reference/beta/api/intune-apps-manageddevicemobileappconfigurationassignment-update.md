---
title: Atualizar managedDeviceMobileAppConfigurationAssignment
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43c4c860c6f0600c7c2877e72fab1a114f0e3329
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974115"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="a1e81-103">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a1e81-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="a1e81-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1e81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1e81-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1e81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1e81-106">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a1e81-106">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1e81-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1e81-107">Prerequisites</span></span>
<span data-ttu-id="a1e81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1e81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e81-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1e81-110">Permission type</span></span>|<span data-ttu-id="a1e81-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1e81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1e81-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1e81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1e81-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1e81-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1e81-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1e81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1e81-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1e81-115">Not supported.</span></span>|
|<span data-ttu-id="a1e81-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1e81-116">Application</span></span>|<span data-ttu-id="a1e81-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1e81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1e81-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1e81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a1e81-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e81-119">Request headers</span></span>
|<span data-ttu-id="a1e81-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1e81-120">Header</span></span>|<span data-ttu-id="a1e81-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1e81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1e81-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1e81-122">Authorization</span></span>|<span data-ttu-id="a1e81-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1e81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1e81-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1e81-124">Accept</span></span>|<span data-ttu-id="a1e81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1e81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1e81-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e81-126">Request body</span></span>
<span data-ttu-id="a1e81-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a1e81-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="a1e81-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a1e81-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="a1e81-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1e81-129">Property</span></span>|<span data-ttu-id="a1e81-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1e81-130">Type</span></span>|<span data-ttu-id="a1e81-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1e81-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1e81-132">id</span><span class="sxs-lookup"><span data-stu-id="a1e81-132">id</span></span>|<span data-ttu-id="a1e81-133">String</span><span class="sxs-lookup"><span data-stu-id="a1e81-133">String</span></span>|<span data-ttu-id="a1e81-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1e81-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="a1e81-135">destino</span><span class="sxs-lookup"><span data-stu-id="a1e81-135">target</span></span>|[<span data-ttu-id="a1e81-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a1e81-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a1e81-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="a1e81-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="a1e81-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e81-138">Response</span></span>
<span data-ttu-id="a1e81-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e81-139">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1e81-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1e81-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1e81-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e81-141">Request</span></span>
<span data-ttu-id="a1e81-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1e81-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="a1e81-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e81-143">Response</span></span>
<span data-ttu-id="a1e81-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1e81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




