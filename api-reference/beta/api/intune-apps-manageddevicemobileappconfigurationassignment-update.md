---
title: Atualizar managedDeviceMobileAppConfigurationAssignment
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0215fdee8754e939d1838ee5c5fd6727d77e5ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935654"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="0158a-103">Atualizar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0158a-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="0158a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0158a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0158a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0158a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0158a-106">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0158a-106">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0158a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0158a-107">Prerequisites</span></span>
<span data-ttu-id="0158a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0158a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0158a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0158a-110">Permission type</span></span>|<span data-ttu-id="0158a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0158a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0158a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0158a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0158a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0158a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0158a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0158a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0158a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0158a-115">Not supported.</span></span>|
|<span data-ttu-id="0158a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0158a-116">Application</span></span>|<span data-ttu-id="0158a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0158a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0158a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0158a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0158a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0158a-119">Request headers</span></span>
|<span data-ttu-id="0158a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0158a-120">Header</span></span>|<span data-ttu-id="0158a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0158a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0158a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0158a-122">Authorization</span></span>|<span data-ttu-id="0158a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0158a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0158a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0158a-124">Accept</span></span>|<span data-ttu-id="0158a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0158a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0158a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0158a-126">Request body</span></span>
<span data-ttu-id="0158a-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0158a-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="0158a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0158a-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="0158a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0158a-129">Property</span></span>|<span data-ttu-id="0158a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0158a-130">Type</span></span>|<span data-ttu-id="0158a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0158a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0158a-132">id</span><span class="sxs-lookup"><span data-stu-id="0158a-132">id</span></span>|<span data-ttu-id="0158a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0158a-133">String</span></span>|<span data-ttu-id="0158a-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="0158a-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0158a-135">destino</span><span class="sxs-lookup"><span data-stu-id="0158a-135">target</span></span>|[<span data-ttu-id="0158a-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0158a-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0158a-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="0158a-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="0158a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0158a-138">Response</span></span>
<span data-ttu-id="0158a-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0158a-139">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0158a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0158a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0158a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0158a-141">Request</span></span>
<span data-ttu-id="0158a-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0158a-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0158a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0158a-143">Response</span></span>
<span data-ttu-id="0158a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0158a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




