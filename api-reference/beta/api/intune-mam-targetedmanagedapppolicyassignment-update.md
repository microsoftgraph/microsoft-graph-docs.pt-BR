---
title: Atualizar targetedManagedAppPolicyAssignment
description: Atualizar as propriedades de um objeto targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 09e2d3685bdfd9fde586612294a386b79bb58f0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858825"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="9db3b-103">Atualizar targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="9db3b-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="9db3b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9db3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9db3b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9db3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9db3b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9db3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9db3b-107">Atualizar as propriedades de um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9db3b-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9db3b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9db3b-108">Prerequisites</span></span>
<span data-ttu-id="9db3b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9db3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9db3b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9db3b-111">Permission type</span></span>|<span data-ttu-id="9db3b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9db3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9db3b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9db3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9db3b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9db3b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9db3b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9db3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9db3b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9db3b-116">Not supported.</span></span>|
|<span data-ttu-id="9db3b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9db3b-117">Application</span></span>|<span data-ttu-id="9db3b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9db3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9db3b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9db3b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9db3b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9db3b-120">Request headers</span></span>
|<span data-ttu-id="9db3b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9db3b-121">Header</span></span>|<span data-ttu-id="9db3b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9db3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9db3b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9db3b-123">Authorization</span></span>|<span data-ttu-id="9db3b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9db3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9db3b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9db3b-125">Accept</span></span>|<span data-ttu-id="9db3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9db3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9db3b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9db3b-127">Request body</span></span>
<span data-ttu-id="9db3b-128">No corpo da solicitação, forneça uma representação JSON do objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9db3b-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="9db3b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9db3b-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="9db3b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9db3b-130">Property</span></span>|<span data-ttu-id="9db3b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9db3b-131">Type</span></span>|<span data-ttu-id="9db3b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9db3b-133">id</span><span class="sxs-lookup"><span data-stu-id="9db3b-133">id</span></span>|<span data-ttu-id="9db3b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9db3b-134">String</span></span>|<span data-ttu-id="9db3b-135">Id</span><span class="sxs-lookup"><span data-stu-id="9db3b-135">Id</span></span>|
|<span data-ttu-id="9db3b-136">destino</span><span class="sxs-lookup"><span data-stu-id="9db3b-136">target</span></span>|[<span data-ttu-id="9db3b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9db3b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9db3b-138">Identificador de implantação de um grupo ou aplicativo</span><span class="sxs-lookup"><span data-stu-id="9db3b-138">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="9db3b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9db3b-139">Response</span></span>
<span data-ttu-id="9db3b-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9db3b-140">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9db3b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9db3b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="9db3b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9db3b-142">Request</span></span>
<span data-ttu-id="9db3b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9db3b-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9db3b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9db3b-144">Response</span></span>
<span data-ttu-id="9db3b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9db3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





