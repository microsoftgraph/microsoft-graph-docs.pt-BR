---
title: Criar deviceCompliancePolicyAssignment
description: Criar um novo objeto deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 752d90ce8f98b69e3f7a429880589f74bccaa82b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805002"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="2caaf-103">Criar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2caaf-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="2caaf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2caaf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2caaf-105">Criar um novo objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2caaf-105">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2caaf-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2caaf-106">Prerequisites</span></span>
<span data-ttu-id="2caaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2caaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2caaf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2caaf-109">Permission type</span></span>|<span data-ttu-id="2caaf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2caaf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2caaf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2caaf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2caaf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2caaf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2caaf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2caaf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2caaf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2caaf-114">Not supported.</span></span>|
|<span data-ttu-id="2caaf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2caaf-115">Application</span></span>|<span data-ttu-id="2caaf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2caaf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2caaf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2caaf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2caaf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2caaf-118">Request headers</span></span>
|<span data-ttu-id="2caaf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2caaf-119">Header</span></span>|<span data-ttu-id="2caaf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2caaf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2caaf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2caaf-121">Authorization</span></span>|<span data-ttu-id="2caaf-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2caaf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2caaf-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2caaf-123">Accept</span></span>|<span data-ttu-id="2caaf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2caaf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2caaf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2caaf-125">Request body</span></span>
<span data-ttu-id="2caaf-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="2caaf-126">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="2caaf-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="2caaf-127">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="2caaf-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2caaf-128">Property</span></span>|<span data-ttu-id="2caaf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2caaf-129">Type</span></span>|<span data-ttu-id="2caaf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2caaf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2caaf-131">id</span><span class="sxs-lookup"><span data-stu-id="2caaf-131">id</span></span>|<span data-ttu-id="2caaf-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2caaf-132">String</span></span>|<span data-ttu-id="2caaf-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2caaf-133">Key of the entity.</span></span>|
|<span data-ttu-id="2caaf-134">destino</span><span class="sxs-lookup"><span data-stu-id="2caaf-134">target</span></span>|[<span data-ttu-id="2caaf-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2caaf-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2caaf-136">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="2caaf-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="2caaf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2caaf-137">Response</span></span>
<span data-ttu-id="2caaf-138">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2caaf-138">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2caaf-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2caaf-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="2caaf-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2caaf-140">Request</span></span>
<span data-ttu-id="2caaf-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2caaf-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2caaf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2caaf-142">Response</span></span>
<span data-ttu-id="2caaf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2caaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



