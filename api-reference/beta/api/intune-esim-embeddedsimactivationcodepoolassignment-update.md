---
title: Atualizar embeddedSIMActivationCodePoolAssignment
description: Atualize as propriedades de um objeto EMBEDDEDSIMActivationCodePoolAssignment incorporado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1fbed18e4b41df0e52e52d50fd73fe89aaf2bda
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126077"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="89e85-103">Atualizar embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="89e85-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

<span data-ttu-id="89e85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89e85-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89e85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89e85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89e85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89e85-107">Atualize as propriedades de [um objeto EMBEDDEDSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) incorporado.</span><span class="sxs-lookup"><span data-stu-id="89e85-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89e85-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89e85-108">Prerequisites</span></span>
<span data-ttu-id="89e85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e85-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89e85-111">Permission type</span></span>|<span data-ttu-id="89e85-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89e85-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89e85-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89e85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89e85-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e85-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89e85-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89e85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89e85-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89e85-116">Not supported.</span></span>|
|<span data-ttu-id="89e85-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89e85-117">Application</span></span>|<span data-ttu-id="89e85-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e85-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89e85-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89e85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="89e85-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89e85-120">Request headers</span></span>
|<span data-ttu-id="89e85-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89e85-121">Header</span></span>|<span data-ttu-id="89e85-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89e85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89e85-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89e85-123">Authorization</span></span>|<span data-ttu-id="89e85-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89e85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89e85-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89e85-125">Accept</span></span>|<span data-ttu-id="89e85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89e85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89e85-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89e85-127">Request body</span></span>
<span data-ttu-id="89e85-128">No corpo da solicitação, fornece uma representação JSON para o [objeto embeddedSIMActivationCodePoolAssignment.](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)</span><span class="sxs-lookup"><span data-stu-id="89e85-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="89e85-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span><span class="sxs-lookup"><span data-stu-id="89e85-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="89e85-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89e85-130">Property</span></span>|<span data-ttu-id="89e85-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="89e85-131">Type</span></span>|<span data-ttu-id="89e85-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="89e85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89e85-133">id</span><span class="sxs-lookup"><span data-stu-id="89e85-133">id</span></span>|<span data-ttu-id="89e85-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89e85-134">String</span></span>|<span data-ttu-id="89e85-135">Identificador exclusivo para a atribuição do pool de código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="89e85-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="89e85-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="89e85-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="89e85-137">destino</span><span class="sxs-lookup"><span data-stu-id="89e85-137">target</span></span>|[<span data-ttu-id="89e85-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="89e85-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="89e85-139">O tipo de grupos direcionados pelo pool de código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="89e85-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="89e85-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e85-140">Response</span></span>
<span data-ttu-id="89e85-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89e85-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89e85-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89e85-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="89e85-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89e85-143">Request</span></span>
<span data-ttu-id="89e85-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89e85-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
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

### <a name="response"></a><span data-ttu-id="89e85-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e85-145">Response</span></span>
<span data-ttu-id="89e85-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89e85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




