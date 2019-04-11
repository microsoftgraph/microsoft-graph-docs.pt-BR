---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abf34960a3f992138094e55a1e6aa3282e7b3d69
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776728"
---
# <a name="assign-action"></a><span data-ttu-id="07dbe-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="07dbe-103">assign action</span></span>

> <span data-ttu-id="07dbe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07dbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07dbe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07dbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07dbe-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07dbe-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07dbe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07dbe-107">Prerequisites</span></span>
<span data-ttu-id="07dbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07dbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07dbe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07dbe-110">Permission type</span></span>|<span data-ttu-id="07dbe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07dbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07dbe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07dbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07dbe-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07dbe-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07dbe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07dbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07dbe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07dbe-115">Not supported.</span></span>|
|<span data-ttu-id="07dbe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07dbe-116">Application</span></span>|<span data-ttu-id="07dbe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07dbe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07dbe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07dbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="07dbe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07dbe-119">Request headers</span></span>
|<span data-ttu-id="07dbe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07dbe-120">Header</span></span>|<span data-ttu-id="07dbe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="07dbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07dbe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07dbe-122">Authorization</span></span>|<span data-ttu-id="07dbe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07dbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07dbe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07dbe-124">Accept</span></span>|<span data-ttu-id="07dbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07dbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07dbe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07dbe-126">Request body</span></span>
<span data-ttu-id="07dbe-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="07dbe-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="07dbe-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="07dbe-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="07dbe-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07dbe-129">Property</span></span>|<span data-ttu-id="07dbe-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="07dbe-130">Type</span></span>|<span data-ttu-id="07dbe-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="07dbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07dbe-132">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="07dbe-132">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="07dbe-133">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="07dbe-133">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="07dbe-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07dbe-134">Not yet documented</span></span>|
|<span data-ttu-id="07dbe-135">assignments</span><span class="sxs-lookup"><span data-stu-id="07dbe-135">assignments</span></span>|<span data-ttu-id="07dbe-136">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="07dbe-136">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="07dbe-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07dbe-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="07dbe-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="07dbe-138">Response</span></span>
<span data-ttu-id="07dbe-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07dbe-139">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07dbe-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07dbe-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="07dbe-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07dbe-141">Request</span></span>
<span data-ttu-id="07dbe-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07dbe-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 548

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
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="07dbe-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="07dbe-143">Response</span></span>
<span data-ttu-id="07dbe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07dbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





