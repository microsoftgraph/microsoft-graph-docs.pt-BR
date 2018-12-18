---
title: Criar managedDeviceMobileAppConfigurationAssignment
description: Criar um novo objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 8418b853c4d82f0a56d592a90542505f0355df0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342774"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="dc86e-103">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="dc86e-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="dc86e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dc86e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc86e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dc86e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc86e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dc86e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc86e-107">Criar um novo objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc86e-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc86e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc86e-108">Prerequisites</span></span>
<span data-ttu-id="dc86e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc86e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc86e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc86e-111">Permission type</span></span>|<span data-ttu-id="dc86e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc86e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc86e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc86e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc86e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc86e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc86e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc86e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc86e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc86e-116">Not supported.</span></span>|
|<span data-ttu-id="dc86e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc86e-117">Application</span></span>|<span data-ttu-id="dc86e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc86e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc86e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc86e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="dc86e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc86e-120">Request headers</span></span>
|<span data-ttu-id="dc86e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc86e-121">Header</span></span>|<span data-ttu-id="dc86e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dc86e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc86e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc86e-123">Authorization</span></span>|<span data-ttu-id="dc86e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc86e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc86e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc86e-125">Accept</span></span>|<span data-ttu-id="dc86e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc86e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc86e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc86e-127">Request body</span></span>
<span data-ttu-id="dc86e-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="dc86e-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="dc86e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="dc86e-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="dc86e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc86e-130">Property</span></span>|<span data-ttu-id="dc86e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc86e-131">Type</span></span>|<span data-ttu-id="dc86e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc86e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc86e-133">id</span><span class="sxs-lookup"><span data-stu-id="dc86e-133">id</span></span>|<span data-ttu-id="dc86e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc86e-134">String</span></span>|<span data-ttu-id="dc86e-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="dc86e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="dc86e-136">destino</span><span class="sxs-lookup"><span data-stu-id="dc86e-136">target</span></span>|[<span data-ttu-id="dc86e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dc86e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dc86e-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="dc86e-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="dc86e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc86e-139">Response</span></span>
<span data-ttu-id="dc86e-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc86e-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc86e-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc86e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc86e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc86e-142">Request</span></span>
<span data-ttu-id="dc86e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc86e-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc86e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc86e-144">Response</span></span>
<span data-ttu-id="dc86e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc86e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





