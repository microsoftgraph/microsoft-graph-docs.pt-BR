---
title: Atualizar embeddedSIMActivationCodePoolAssignment
description: Atualiza as propriedades de um objeto embeddedSIMActivationCodePoolAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 601813bb791cfe97da52db41a2c6a49d706a8452
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995234"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="58ab5-103">Atualizar embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="58ab5-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="58ab5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58ab5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58ab5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58ab5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58ab5-106">Atualiza as propriedades de um objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="58ab5-106">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58ab5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58ab5-107">Prerequisites</span></span>
<span data-ttu-id="58ab5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58ab5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58ab5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58ab5-110">Permission type</span></span>|<span data-ttu-id="58ab5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58ab5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58ab5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58ab5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58ab5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58ab5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58ab5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58ab5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58ab5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58ab5-115">Not supported.</span></span>|
|<span data-ttu-id="58ab5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58ab5-116">Application</span></span>|<span data-ttu-id="58ab5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58ab5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58ab5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58ab5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="58ab5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58ab5-119">Request headers</span></span>
|<span data-ttu-id="58ab5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58ab5-120">Header</span></span>|<span data-ttu-id="58ab5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58ab5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58ab5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58ab5-122">Authorization</span></span>|<span data-ttu-id="58ab5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58ab5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58ab5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58ab5-124">Accept</span></span>|<span data-ttu-id="58ab5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58ab5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58ab5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58ab5-126">Request body</span></span>
<span data-ttu-id="58ab5-127">No corpo da solicitação, forneça uma representação JSON do objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="58ab5-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="58ab5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span><span class="sxs-lookup"><span data-stu-id="58ab5-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="58ab5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58ab5-129">Property</span></span>|<span data-ttu-id="58ab5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="58ab5-130">Type</span></span>|<span data-ttu-id="58ab5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="58ab5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58ab5-132">id</span><span class="sxs-lookup"><span data-stu-id="58ab5-132">id</span></span>|<span data-ttu-id="58ab5-133">String</span><span class="sxs-lookup"><span data-stu-id="58ab5-133">String</span></span>|<span data-ttu-id="58ab5-134">Identificador exclusivo da atribuição do pool de códigos de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="58ab5-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="58ab5-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="58ab5-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="58ab5-136">destino</span><span class="sxs-lookup"><span data-stu-id="58ab5-136">target</span></span>|[<span data-ttu-id="58ab5-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="58ab5-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="58ab5-138">O tipo de grupos direcionados pelo pool de códigos de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="58ab5-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="58ab5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="58ab5-139">Response</span></span>
<span data-ttu-id="58ab5-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58ab5-140">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58ab5-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58ab5-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="58ab5-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58ab5-142">Request</span></span>
<span data-ttu-id="58ab5-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58ab5-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="58ab5-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="58ab5-144">Response</span></span>
<span data-ttu-id="58ab5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58ab5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





