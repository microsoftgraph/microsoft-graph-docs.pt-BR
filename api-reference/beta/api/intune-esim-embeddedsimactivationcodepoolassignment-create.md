---
title: Criar embeddedSIMActivationCodePoolAssignment
description: Criar um novo objeto embeddedSIMActivationCodePoolAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b836930a12abb78c0640ef508a62945b8c017fe9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792019"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="6e568-103">Criar embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="6e568-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

<span data-ttu-id="6e568-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e568-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e568-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e568-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e568-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e568-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e568-107">Criar um novo objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6e568-107">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e568-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e568-108">Prerequisites</span></span>
<span data-ttu-id="6e568-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6e568-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6e568-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e568-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e568-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e568-111">Permission type</span></span>|<span data-ttu-id="6e568-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e568-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e568-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e568-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e568-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e568-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e568-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e568-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e568-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e568-116">Not supported.</span></span>|
|<span data-ttu-id="6e568-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e568-117">Application</span></span>|<span data-ttu-id="6e568-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e568-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e568-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e568-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6e568-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e568-120">Request headers</span></span>
|<span data-ttu-id="6e568-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e568-121">Header</span></span>|<span data-ttu-id="6e568-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e568-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e568-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e568-123">Authorization</span></span>|<span data-ttu-id="6e568-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e568-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e568-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e568-125">Accept</span></span>|<span data-ttu-id="6e568-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e568-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e568-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e568-127">Request body</span></span>
<span data-ttu-id="6e568-128">No corpo da solicitação, forneça uma representação JSON do objeto embeddedSIMActivationCodePoolAssignment.</span><span class="sxs-lookup"><span data-stu-id="6e568-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="6e568-129">A tabela a seguir mostra as propriedades que são necessárias ao criar embeddedSIMActivationCodePoolAssignment.</span><span class="sxs-lookup"><span data-stu-id="6e568-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="6e568-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e568-130">Property</span></span>|<span data-ttu-id="6e568-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e568-131">Type</span></span>|<span data-ttu-id="6e568-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e568-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e568-133">id</span><span class="sxs-lookup"><span data-stu-id="6e568-133">id</span></span>|<span data-ttu-id="6e568-134">String</span><span class="sxs-lookup"><span data-stu-id="6e568-134">String</span></span>|<span data-ttu-id="6e568-135">Identificador exclusivo da atribuição do pool de códigos de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="6e568-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="6e568-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="6e568-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="6e568-137">destino</span><span class="sxs-lookup"><span data-stu-id="6e568-137">target</span></span>|[<span data-ttu-id="6e568-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6e568-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6e568-139">O tipo de grupos direcionados pelo pool de códigos de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="6e568-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="6e568-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e568-140">Response</span></span>
<span data-ttu-id="6e568-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e568-141">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e568-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e568-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e568-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e568-143">Request</span></span>
<span data-ttu-id="6e568-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e568-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 340

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="6e568-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e568-145">Response</span></span>
<span data-ttu-id="6e568-146">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6e568-146">Here is an example of the response.</span></span> <span data-ttu-id="6e568-147">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6e568-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6e568-148">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6e568-148">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



