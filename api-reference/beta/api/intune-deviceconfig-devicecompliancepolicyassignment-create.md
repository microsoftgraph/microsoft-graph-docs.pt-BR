---
title: Criar deviceCompliancePolicyAssignment
description: Criar um novo objeto deviceCompliancePolicyAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3fb7372bf769366ef83999a82461ce0cc6563066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414904"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="2986c-103">Criar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="2986c-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="2986c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2986c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2986c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2986c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2986c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2986c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2986c-107">Criar um novo objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2986c-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2986c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2986c-108">Prerequisites</span></span>
<span data-ttu-id="2986c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2986c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2986c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2986c-111">Permission type</span></span>|<span data-ttu-id="2986c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2986c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2986c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2986c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2986c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2986c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2986c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2986c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2986c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2986c-116">Not supported.</span></span>|
|<span data-ttu-id="2986c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2986c-117">Application</span></span>|<span data-ttu-id="2986c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2986c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2986c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2986c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2986c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2986c-120">Request headers</span></span>
|<span data-ttu-id="2986c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2986c-121">Header</span></span>|<span data-ttu-id="2986c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2986c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2986c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2986c-123">Authorization</span></span>|<span data-ttu-id="2986c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2986c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2986c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2986c-125">Accept</span></span>|<span data-ttu-id="2986c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2986c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2986c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2986c-127">Request body</span></span>
<span data-ttu-id="2986c-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="2986c-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="2986c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="2986c-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="2986c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2986c-130">Property</span></span>|<span data-ttu-id="2986c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2986c-131">Type</span></span>|<span data-ttu-id="2986c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2986c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2986c-133">id</span><span class="sxs-lookup"><span data-stu-id="2986c-133">id</span></span>|<span data-ttu-id="2986c-134">String</span><span class="sxs-lookup"><span data-stu-id="2986c-134">String</span></span>|<span data-ttu-id="2986c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2986c-135">Key of the entity.</span></span>|
|<span data-ttu-id="2986c-136">destino</span><span class="sxs-lookup"><span data-stu-id="2986c-136">target</span></span>|[<span data-ttu-id="2986c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2986c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2986c-138">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="2986c-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="2986c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2986c-139">Response</span></span>
<span data-ttu-id="2986c-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2986c-140">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2986c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2986c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2986c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2986c-142">Request</span></span>
<span data-ttu-id="2986c-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2986c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2986c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2986c-144">Response</span></span>
<span data-ttu-id="2986c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2986c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




