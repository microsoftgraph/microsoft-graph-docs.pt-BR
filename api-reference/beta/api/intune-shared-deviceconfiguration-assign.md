---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd0ff2b512d3b86d7153689dbb9b76e2ff5f5ef4
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086162"
---
# <a name="assign-action"></a><span data-ttu-id="ee8b6-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="ee8b6-103">assign action</span></span>

> <span data-ttu-id="ee8b6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee8b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee8b6-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ee8b6-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee8b6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee8b6-107">Prerequisites</span></span>
<span data-ttu-id="ee8b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee8b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee8b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee8b6-110">Permission type</span></span>|<span data-ttu-id="ee8b6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee8b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee8b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee8b6-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ee8b6-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ee8b6-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ee8b6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee8b6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee8b6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee8b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee8b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-116">Not supported.</span></span>|
|<span data-ttu-id="ee8b6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee8b6-117">Application</span></span>||
| <span data-ttu-id="ee8b6-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ee8b6-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ee8b6-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee8b6-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee8b6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee8b6-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ee8b6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee8b6-121">Request headers</span></span>
|<span data-ttu-id="ee8b6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee8b6-122">Header</span></span>|<span data-ttu-id="ee8b6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ee8b6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee8b6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee8b6-124">Authorization</span></span>|<span data-ttu-id="ee8b6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee8b6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee8b6-126">Accept</span></span>|<span data-ttu-id="ee8b6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ee8b6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee8b6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee8b6-128">Request body</span></span>
<span data-ttu-id="ee8b6-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ee8b6-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ee8b6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee8b6-131">Property</span></span>|<span data-ttu-id="ee8b6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee8b6-132">Type</span></span>|<span data-ttu-id="ee8b6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee8b6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee8b6-134">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="ee8b6-134">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="ee8b6-135">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ee8b6-135">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="ee8b6-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ee8b6-136">Not yet documented</span></span>|
|<span data-ttu-id="ee8b6-137">assignments</span><span class="sxs-lookup"><span data-stu-id="ee8b6-137">assignments</span></span>|<span data-ttu-id="ee8b6-138">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ee8b6-138">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ee8b6-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ee8b6-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ee8b6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee8b6-140">Response</span></span>
<span data-ttu-id="ee8b6-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-141">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee8b6-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee8b6-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee8b6-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee8b6-143">Request</span></span>
<span data-ttu-id="ee8b6-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 617

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ee8b6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee8b6-145">Response</span></span>
<span data-ttu-id="ee8b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee8b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```









