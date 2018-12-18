---
title: Atualizar deviceCompliancePolicyAssignment
description: Atualizar as propriedades de um objeto deviceCompliancePolicyAssignment.
author: tfitzmac
ms.openlocfilehash: 3c968232fdcc629376e5d7cc22758dd626d7f2a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327234"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="ed35f-103">Atualizar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ed35f-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="ed35f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed35f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed35f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed35f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed35f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed35f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed35f-107">Atualizar as propriedades de um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ed35f-107">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed35f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed35f-108">Prerequisites</span></span>
<span data-ttu-id="ed35f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed35f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed35f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed35f-111">Permission type</span></span>|<span data-ttu-id="ed35f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed35f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed35f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed35f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed35f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed35f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed35f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed35f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed35f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed35f-116">Not supported.</span></span>|
|<span data-ttu-id="ed35f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed35f-117">Application</span></span>|<span data-ttu-id="ed35f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed35f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed35f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed35f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ed35f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed35f-120">Request headers</span></span>
|<span data-ttu-id="ed35f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed35f-121">Header</span></span>|<span data-ttu-id="ed35f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ed35f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed35f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed35f-123">Authorization</span></span>|<span data-ttu-id="ed35f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed35f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed35f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed35f-125">Accept</span></span>|<span data-ttu-id="ed35f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed35f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed35f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed35f-127">Request body</span></span>
<span data-ttu-id="ed35f-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ed35f-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="ed35f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ed35f-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="ed35f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed35f-130">Property</span></span>|<span data-ttu-id="ed35f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed35f-131">Type</span></span>|<span data-ttu-id="ed35f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed35f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed35f-133">id</span><span class="sxs-lookup"><span data-stu-id="ed35f-133">id</span></span>|<span data-ttu-id="ed35f-134">String</span><span class="sxs-lookup"><span data-stu-id="ed35f-134">String</span></span>|<span data-ttu-id="ed35f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ed35f-135">Key of the entity.</span></span>|
|<span data-ttu-id="ed35f-136">destino</span><span class="sxs-lookup"><span data-stu-id="ed35f-136">target</span></span>|[<span data-ttu-id="ed35f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ed35f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ed35f-138">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="ed35f-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ed35f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed35f-139">Response</span></span>
<span data-ttu-id="ed35f-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed35f-140">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed35f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed35f-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed35f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed35f-142">Request</span></span>
<span data-ttu-id="ed35f-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed35f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ed35f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed35f-144">Response</span></span>
<span data-ttu-id="ed35f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed35f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





