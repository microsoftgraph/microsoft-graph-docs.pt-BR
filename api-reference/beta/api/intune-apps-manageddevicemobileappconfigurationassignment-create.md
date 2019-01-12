---
title: Criar managedDeviceMobileAppConfigurationAssignment
description: Criar um novo objeto managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 08f672c76b7cd0e044ac0a309dd1a770f15d03c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945780"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="96e39-103">Criar managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="96e39-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="96e39-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96e39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96e39-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96e39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96e39-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96e39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96e39-107">Criar um novo objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96e39-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96e39-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96e39-108">Prerequisites</span></span>
<span data-ttu-id="96e39-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96e39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e39-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96e39-111">Permission type</span></span>|<span data-ttu-id="96e39-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96e39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96e39-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96e39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96e39-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e39-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96e39-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96e39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96e39-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96e39-116">Not supported.</span></span>|
|<span data-ttu-id="96e39-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96e39-117">Application</span></span>|<span data-ttu-id="96e39-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96e39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96e39-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96e39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="96e39-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96e39-120">Request headers</span></span>
|<span data-ttu-id="96e39-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96e39-121">Header</span></span>|<span data-ttu-id="96e39-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96e39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96e39-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96e39-123">Authorization</span></span>|<span data-ttu-id="96e39-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96e39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96e39-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96e39-125">Accept</span></span>|<span data-ttu-id="96e39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96e39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96e39-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96e39-127">Request body</span></span>
<span data-ttu-id="96e39-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="96e39-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="96e39-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="96e39-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="96e39-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96e39-130">Property</span></span>|<span data-ttu-id="96e39-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="96e39-131">Type</span></span>|<span data-ttu-id="96e39-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="96e39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96e39-133">id</span><span class="sxs-lookup"><span data-stu-id="96e39-133">id</span></span>|<span data-ttu-id="96e39-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96e39-134">String</span></span>|<span data-ttu-id="96e39-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="96e39-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="96e39-136">destino</span><span class="sxs-lookup"><span data-stu-id="96e39-136">target</span></span>|[<span data-ttu-id="96e39-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="96e39-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="96e39-138">Destino de atribuição ao qual a política de T&C foi designada.</span><span class="sxs-lookup"><span data-stu-id="96e39-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="96e39-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e39-139">Response</span></span>
<span data-ttu-id="96e39-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96e39-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96e39-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96e39-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="96e39-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96e39-142">Request</span></span>
<span data-ttu-id="96e39-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96e39-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96e39-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e39-144">Response</span></span>
<span data-ttu-id="96e39-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96e39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





