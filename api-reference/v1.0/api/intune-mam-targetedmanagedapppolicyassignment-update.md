---
title: Atualizar targetedManagedAppPolicyAssignment
description: Atualizar as propriedades de um objeto targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5d20413017c9a1063204273574bb9b24e8ba31b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927762"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="ddd8a-103">Atualizar targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ddd8a-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="ddd8a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ddd8a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddd8a-105">Atualizar as propriedades de um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ddd8a-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddd8a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ddd8a-106">Prerequisites</span></span>
<span data-ttu-id="ddd8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddd8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd8a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddd8a-109">Permission type</span></span>|<span data-ttu-id="ddd8a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ddd8a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddd8a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddd8a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ddd8a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddd8a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ddd8a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddd8a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddd8a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddd8a-114">Not supported.</span></span>|
|<span data-ttu-id="ddd8a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddd8a-115">Application</span></span>|<span data-ttu-id="ddd8a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddd8a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddd8a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddd8a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ddd8a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd8a-118">Request headers</span></span>
|<span data-ttu-id="ddd8a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddd8a-119">Header</span></span>|<span data-ttu-id="ddd8a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ddd8a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddd8a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddd8a-121">Authorization</span></span>|<span data-ttu-id="ddd8a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddd8a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddd8a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ddd8a-123">Accept</span></span>|<span data-ttu-id="ddd8a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ddd8a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddd8a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd8a-125">Request body</span></span>
<span data-ttu-id="ddd8a-126">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ddd8a-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="ddd8a-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ddd8a-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="ddd8a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddd8a-128">Property</span></span>|<span data-ttu-id="ddd8a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddd8a-129">Type</span></span>|<span data-ttu-id="ddd8a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddd8a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd8a-131">id</span><span class="sxs-lookup"><span data-stu-id="ddd8a-131">id</span></span>|<span data-ttu-id="ddd8a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddd8a-132">String</span></span>|<span data-ttu-id="ddd8a-133">Id</span><span class="sxs-lookup"><span data-stu-id="ddd8a-133">Id</span></span>|
|<span data-ttu-id="ddd8a-134">destino</span><span class="sxs-lookup"><span data-stu-id="ddd8a-134">target</span></span>|[<span data-ttu-id="ddd8a-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ddd8a-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ddd8a-136">Identificador de implantação de um grupo ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddd8a-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="ddd8a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddd8a-137">Response</span></span>
<span data-ttu-id="ddd8a-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddd8a-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd8a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddd8a-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddd8a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd8a-140">Request</span></span>
<span data-ttu-id="ddd8a-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddd8a-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ddd8a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddd8a-142">Response</span></span>
<span data-ttu-id="ddd8a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddd8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



