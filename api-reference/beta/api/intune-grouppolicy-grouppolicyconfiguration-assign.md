---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00431a77432738eca351ccbe04d1a06c289db806
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791991"
---
# <a name="assign-action"></a><span data-ttu-id="5fbf0-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="5fbf0-103">assign action</span></span>

<span data-ttu-id="5fbf0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fbf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5fbf0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fbf0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fbf0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5fbf0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fbf0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5fbf0-108">Prerequisites</span></span>
<span data-ttu-id="5fbf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fbf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fbf0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fbf0-111">Permission type</span></span>|<span data-ttu-id="5fbf0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5fbf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fbf0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fbf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5fbf0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fbf0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5fbf0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fbf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fbf0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-116">Not supported.</span></span>|
|<span data-ttu-id="5fbf0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fbf0-117">Application</span></span>|<span data-ttu-id="5fbf0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fbf0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fbf0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fbf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5fbf0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbf0-120">Request headers</span></span>
|<span data-ttu-id="5fbf0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5fbf0-121">Header</span></span>|<span data-ttu-id="5fbf0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5fbf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fbf0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fbf0-123">Authorization</span></span>|<span data-ttu-id="5fbf0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fbf0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5fbf0-125">Accept</span></span>|<span data-ttu-id="5fbf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fbf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fbf0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbf0-127">Request body</span></span>
<span data-ttu-id="5fbf0-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5fbf0-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5fbf0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fbf0-130">Property</span></span>|<span data-ttu-id="5fbf0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fbf0-131">Type</span></span>|<span data-ttu-id="5fbf0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fbf0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fbf0-133">assignments</span><span class="sxs-lookup"><span data-stu-id="5fbf0-133">assignments</span></span>|<span data-ttu-id="5fbf0-134">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5fbf0-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5fbf0-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5fbf0-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5fbf0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fbf0-136">Response</span></span>
<span data-ttu-id="5fbf0-137">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-137">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fbf0-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fbf0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fbf0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbf0-139">Request</span></span>
<span data-ttu-id="5fbf0-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 513

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5fbf0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fbf0-141">Response</span></span>
<span data-ttu-id="5fbf0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fbf0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 507

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



