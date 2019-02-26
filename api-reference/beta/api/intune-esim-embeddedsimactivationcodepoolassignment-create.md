---
title: Criar embeddedSIMActivationCodePoolAssignment
description: Criar um novo objeto embeddedSIMActivationCodePoolAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02b4c39b4ca999780a620510c38fc80036e02ee1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169619"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="44fbb-103">Criar embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="44fbb-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="44fbb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44fbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44fbb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44fbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44fbb-106">Criar um novo objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="44fbb-106">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44fbb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44fbb-107">Prerequisites</span></span>
<span data-ttu-id="44fbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="44fbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44fbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44fbb-110">Permission type</span></span>|<span data-ttu-id="44fbb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44fbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44fbb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44fbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44fbb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44fbb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44fbb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44fbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44fbb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44fbb-115">Not supported.</span></span>|
|<span data-ttu-id="44fbb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44fbb-116">Application</span></span>|<span data-ttu-id="44fbb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44fbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44fbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44fbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="44fbb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44fbb-119">Request headers</span></span>
|<span data-ttu-id="44fbb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44fbb-120">Header</span></span>|<span data-ttu-id="44fbb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="44fbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44fbb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="44fbb-122">Authorization</span></span>|<span data-ttu-id="44fbb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44fbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44fbb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44fbb-124">Accept</span></span>|<span data-ttu-id="44fbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44fbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44fbb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44fbb-126">Request body</span></span>
<span data-ttu-id="44fbb-127">No corpo da solicitação, forneça uma representação JSON do objeto embeddedSIMActivationCodePoolAssignment.</span><span class="sxs-lookup"><span data-stu-id="44fbb-127">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="44fbb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar embeddedSIMActivationCodePoolAssignment.</span><span class="sxs-lookup"><span data-stu-id="44fbb-128">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="44fbb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44fbb-129">Property</span></span>|<span data-ttu-id="44fbb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44fbb-130">Type</span></span>|<span data-ttu-id="44fbb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44fbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44fbb-132">id</span><span class="sxs-lookup"><span data-stu-id="44fbb-132">id</span></span>|<span data-ttu-id="44fbb-133">String</span><span class="sxs-lookup"><span data-stu-id="44fbb-133">String</span></span>|<span data-ttu-id="44fbb-134">Identificador exclusivo da atribuição do pool de códigos de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="44fbb-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="44fbb-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="44fbb-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="44fbb-136">destino</span><span class="sxs-lookup"><span data-stu-id="44fbb-136">target</span></span>|[<span data-ttu-id="44fbb-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="44fbb-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="44fbb-138">O tipo de grupos direcionados pelo pool de códigos de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="44fbb-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="44fbb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="44fbb-139">Response</span></span>
<span data-ttu-id="44fbb-140">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44fbb-140">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44fbb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44fbb-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="44fbb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44fbb-142">Request</span></span>
<span data-ttu-id="44fbb-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44fbb-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="44fbb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="44fbb-144">Response</span></span>
<span data-ttu-id="44fbb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44fbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




