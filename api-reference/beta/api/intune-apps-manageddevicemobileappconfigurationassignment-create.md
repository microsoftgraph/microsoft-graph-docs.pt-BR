---
title: Criar managedDeviceMobileAppConfigurationAssignment
description: Criar um novo objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46be79632e172ee1f188fd0daeee2edd1b493626
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161303"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="29081-103">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="29081-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="29081-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29081-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29081-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29081-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29081-106">Criar um novo objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="29081-106">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29081-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29081-107">Prerequisites</span></span>
<span data-ttu-id="29081-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="29081-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="29081-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29081-110">Permission type</span></span>|<span data-ttu-id="29081-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29081-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29081-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29081-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29081-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29081-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="29081-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29081-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29081-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29081-115">Not supported.</span></span>|
|<span data-ttu-id="29081-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29081-116">Application</span></span>|<span data-ttu-id="29081-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29081-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29081-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29081-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="29081-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29081-119">Request headers</span></span>
|<span data-ttu-id="29081-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29081-120">Header</span></span>|<span data-ttu-id="29081-121">Valor</span><span class="sxs-lookup"><span data-stu-id="29081-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29081-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="29081-122">Authorization</span></span>|<span data-ttu-id="29081-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29081-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29081-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29081-124">Accept</span></span>|<span data-ttu-id="29081-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29081-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29081-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29081-126">Request body</span></span>
<span data-ttu-id="29081-127">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="29081-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="29081-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="29081-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="29081-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29081-129">Property</span></span>|<span data-ttu-id="29081-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="29081-130">Type</span></span>|<span data-ttu-id="29081-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="29081-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29081-132">id</span><span class="sxs-lookup"><span data-stu-id="29081-132">id</span></span>|<span data-ttu-id="29081-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29081-133">String</span></span>|<span data-ttu-id="29081-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="29081-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="29081-135">destino</span><span class="sxs-lookup"><span data-stu-id="29081-135">target</span></span>|[<span data-ttu-id="29081-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="29081-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="29081-137">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="29081-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="29081-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="29081-138">Response</span></span>
<span data-ttu-id="29081-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29081-139">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29081-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29081-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="29081-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29081-141">Request</span></span>
<span data-ttu-id="29081-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29081-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="29081-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="29081-143">Response</span></span>
<span data-ttu-id="29081-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29081-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




