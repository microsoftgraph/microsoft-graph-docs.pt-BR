---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b7117abada0216a9fc1252769a4bc02287fb287
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129276"
---
# <a name="assign-action"></a><span data-ttu-id="8ed6f-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="8ed6f-103">assign action</span></span>

<span data-ttu-id="8ed6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ed6f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ed6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ed6f-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8ed6f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ed6f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ed6f-108">Prerequisites</span></span>
<span data-ttu-id="8ed6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ed6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ed6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ed6f-111">Permission type</span></span>|<span data-ttu-id="8ed6f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ed6f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ed6f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ed6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ed6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ed6f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ed6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ed6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-116">Not supported.</span></span>|
|<span data-ttu-id="8ed6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ed6f-117">Application</span></span>|<span data-ttu-id="8ed6f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed6f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ed6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="8ed6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6f-120">Request headers</span></span>
|<span data-ttu-id="8ed6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ed6f-121">Header</span></span>|<span data-ttu-id="8ed6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8ed6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ed6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ed6f-123">Authorization</span></span>|<span data-ttu-id="8ed6f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ed6f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ed6f-125">Accept</span></span>|<span data-ttu-id="8ed6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ed6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ed6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6f-127">Request body</span></span>
<span data-ttu-id="8ed6f-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8ed6f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8ed6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ed6f-130">Property</span></span>|<span data-ttu-id="8ed6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ed6f-131">Type</span></span>|<span data-ttu-id="8ed6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ed6f-133">assignments</span><span class="sxs-lookup"><span data-stu-id="8ed6f-133">assignments</span></span>|<span data-ttu-id="8ed6f-134">[Coleção deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8ed6f-134">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="8ed6f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8ed6f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8ed6f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed6f-136">Response</span></span>
<span data-ttu-id="8ed6f-137">Se tiver êxito, essa ação retornará um código de resposta e uma coleção `200 OK` [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-137">If successful, this action returns a `200 OK` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ed6f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ed6f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ed6f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6f-139">Request</span></span>
<span data-ttu-id="8ed6f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assign

Content-type: application/json
Content-length: 524

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
      "id": "1f069921-9921-1f06-2199-061f2199061f",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="8ed6f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed6f-141">Response</span></span>
<span data-ttu-id="8ed6f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ed6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
      "id": "1f069921-9921-1f06-2199-061f2199061f",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




