---
title: Atualizar deviceCompliancePolicyAssignment
description: Atualizar as propriedades de um objeto deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b86a3e338574aa97f463a9c7a52b41a5fea1e4b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868793"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="a0939-103">Atualizar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a0939-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="a0939-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0939-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0939-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0939-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0939-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0939-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0939-107">Atualizar as propriedades de um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0939-107">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0939-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0939-108">Prerequisites</span></span>
<span data-ttu-id="a0939-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0939-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0939-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0939-111">Permission type</span></span>|<span data-ttu-id="a0939-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0939-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0939-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0939-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0939-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0939-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0939-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0939-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0939-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0939-116">Not supported.</span></span>|
|<span data-ttu-id="a0939-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0939-117">Application</span></span>|<span data-ttu-id="a0939-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0939-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0939-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0939-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a0939-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0939-120">Request headers</span></span>
|<span data-ttu-id="a0939-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0939-121">Header</span></span>|<span data-ttu-id="a0939-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0939-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0939-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0939-123">Authorization</span></span>|<span data-ttu-id="a0939-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0939-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0939-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0939-125">Accept</span></span>|<span data-ttu-id="a0939-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0939-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0939-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0939-127">Request body</span></span>
<span data-ttu-id="a0939-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0939-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="a0939-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0939-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="a0939-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0939-130">Property</span></span>|<span data-ttu-id="a0939-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0939-131">Type</span></span>|<span data-ttu-id="a0939-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0939-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0939-133">id</span><span class="sxs-lookup"><span data-stu-id="a0939-133">id</span></span>|<span data-ttu-id="a0939-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0939-134">String</span></span>|<span data-ttu-id="a0939-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0939-135">Key of the entity.</span></span>|
|<span data-ttu-id="a0939-136">destino</span><span class="sxs-lookup"><span data-stu-id="a0939-136">target</span></span>|[<span data-ttu-id="a0939-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a0939-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a0939-138">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="a0939-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="a0939-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0939-139">Response</span></span>
<span data-ttu-id="a0939-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0939-140">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0939-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0939-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0939-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0939-142">Request</span></span>
<span data-ttu-id="a0939-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0939-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0939-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0939-144">Response</span></span>
<span data-ttu-id="a0939-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0939-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





