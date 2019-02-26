---
title: Criar managedDeviceMobileAppConfigurationAssignment
description: Criar um novo objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 590b6b841a528806f4dccd0357ce0529be6e1a77
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253747"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="59dfb-103">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="59dfb-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="59dfb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59dfb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59dfb-105">Criar um novo objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="59dfb-105">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59dfb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59dfb-106">Prerequisites</span></span>
<span data-ttu-id="59dfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="59dfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="59dfb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59dfb-109">Permission type</span></span>|<span data-ttu-id="59dfb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59dfb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59dfb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59dfb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59dfb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59dfb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59dfb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59dfb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59dfb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59dfb-114">Not supported.</span></span>|
|<span data-ttu-id="59dfb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59dfb-115">Application</span></span>|<span data-ttu-id="59dfb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59dfb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59dfb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59dfb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="59dfb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59dfb-118">Request headers</span></span>
|<span data-ttu-id="59dfb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59dfb-119">Header</span></span>|<span data-ttu-id="59dfb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="59dfb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59dfb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="59dfb-121">Authorization</span></span>|<span data-ttu-id="59dfb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59dfb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59dfb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59dfb-123">Accept</span></span>|<span data-ttu-id="59dfb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="59dfb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59dfb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59dfb-125">Request body</span></span>
<span data-ttu-id="59dfb-126">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="59dfb-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="59dfb-127">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="59dfb-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="59dfb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59dfb-128">Property</span></span>|<span data-ttu-id="59dfb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="59dfb-129">Type</span></span>|<span data-ttu-id="59dfb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="59dfb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59dfb-131">id</span><span class="sxs-lookup"><span data-stu-id="59dfb-131">id</span></span>|<span data-ttu-id="59dfb-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59dfb-132">String</span></span>|<span data-ttu-id="59dfb-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="59dfb-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="59dfb-134">destino</span><span class="sxs-lookup"><span data-stu-id="59dfb-134">target</span></span>|[<span data-ttu-id="59dfb-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="59dfb-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="59dfb-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="59dfb-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="59dfb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="59dfb-137">Response</span></span>
<span data-ttu-id="59dfb-138">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59dfb-138">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59dfb-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59dfb-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="59dfb-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59dfb-140">Request</span></span>
<span data-ttu-id="59dfb-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59dfb-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="59dfb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="59dfb-142">Response</span></span>
<span data-ttu-id="59dfb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59dfb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



