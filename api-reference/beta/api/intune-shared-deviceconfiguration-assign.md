---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bdaece991a477a3323919f4baf275b409b2cc0bc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863335"
---
# <a name="assign-action"></a><span data-ttu-id="97252-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="97252-103">assign action</span></span>

<span data-ttu-id="97252-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97252-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97252-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97252-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97252-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97252-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97252-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97252-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97252-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97252-108">Prerequisites</span></span>
<span data-ttu-id="97252-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97252-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97252-111">Permission type</span></span>|<span data-ttu-id="97252-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97252-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97252-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97252-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="97252-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="97252-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="97252-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97252-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97252-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97252-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97252-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97252-117">Not supported.</span></span>|
|<span data-ttu-id="97252-118">Application</span><span class="sxs-lookup"><span data-stu-id="97252-118">Application</span></span>||
| <span data-ttu-id="97252-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="97252-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="97252-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97252-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97252-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97252-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="97252-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97252-122">Request headers</span></span>
|<span data-ttu-id="97252-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97252-123">Header</span></span>|<span data-ttu-id="97252-124">Valor</span><span class="sxs-lookup"><span data-stu-id="97252-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97252-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="97252-125">Authorization</span></span>|<span data-ttu-id="97252-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97252-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97252-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97252-127">Accept</span></span>|<span data-ttu-id="97252-128">application/json</span><span class="sxs-lookup"><span data-stu-id="97252-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97252-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97252-129">Request body</span></span>
<span data-ttu-id="97252-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="97252-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="97252-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="97252-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="97252-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97252-132">Property</span></span>|<span data-ttu-id="97252-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="97252-133">Type</span></span>|<span data-ttu-id="97252-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="97252-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97252-135">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="97252-135">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="97252-136">[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="97252-136">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="97252-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97252-137">Not yet documented</span></span>|
|<span data-ttu-id="97252-138">assignments</span><span class="sxs-lookup"><span data-stu-id="97252-138">assignments</span></span>|<span data-ttu-id="97252-139">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="97252-139">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="97252-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="97252-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="97252-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="97252-141">Response</span></span>
<span data-ttu-id="97252-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97252-142">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97252-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97252-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="97252-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97252-144">Request</span></span>
<span data-ttu-id="97252-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97252-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97252-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="97252-146">Response</span></span>
<span data-ttu-id="97252-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97252-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







