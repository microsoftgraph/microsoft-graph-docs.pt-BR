---
title: Criar managedDeviceMobileAppConfigurationAssignment
description: Criar um novo objeto managedDeviceMobileAppConfigurationAssignment.
ms.openlocfilehash: 4b479f7c0f93e41aa8691749925203652d2dcc9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004560"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="85219-103">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="85219-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="85219-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="85219-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85219-105">Criar um novo objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="85219-105">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85219-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85219-106">Prerequisites</span></span>
<span data-ttu-id="85219-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85219-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85219-109">Permission type</span></span>|<span data-ttu-id="85219-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85219-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85219-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85219-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85219-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85219-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85219-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85219-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85219-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85219-114">Not supported.</span></span>|
|<span data-ttu-id="85219-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85219-115">Application</span></span>|<span data-ttu-id="85219-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85219-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85219-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85219-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="85219-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85219-118">Request headers</span></span>
|<span data-ttu-id="85219-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85219-119">Header</span></span>|<span data-ttu-id="85219-120">Valor</span><span class="sxs-lookup"><span data-stu-id="85219-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85219-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="85219-121">Authorization</span></span>|<span data-ttu-id="85219-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85219-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85219-123">Accept</span><span class="sxs-lookup"><span data-stu-id="85219-123">Accept</span></span>|<span data-ttu-id="85219-124">application/json</span><span class="sxs-lookup"><span data-stu-id="85219-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85219-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85219-125">Request body</span></span>
<span data-ttu-id="85219-126">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="85219-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="85219-127">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="85219-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="85219-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85219-128">Property</span></span>|<span data-ttu-id="85219-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="85219-129">Type</span></span>|<span data-ttu-id="85219-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="85219-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85219-131">id</span><span class="sxs-lookup"><span data-stu-id="85219-131">id</span></span>|<span data-ttu-id="85219-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85219-132">String</span></span>|<span data-ttu-id="85219-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="85219-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="85219-134">destino</span><span class="sxs-lookup"><span data-stu-id="85219-134">target</span></span>|[<span data-ttu-id="85219-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="85219-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="85219-136">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="85219-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="85219-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="85219-137">Response</span></span>
<span data-ttu-id="85219-138">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85219-138">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85219-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85219-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="85219-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85219-140">Request</span></span>
<span data-ttu-id="85219-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85219-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85219-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="85219-142">Response</span></span>
<span data-ttu-id="85219-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85219-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



