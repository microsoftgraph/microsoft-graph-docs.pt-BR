---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b078d917482bc1d62c51f9e1d3d9008d94d8432f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156564"
---
# <a name="assign-action"></a><span data-ttu-id="f8931-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="f8931-103">assign action</span></span>

<span data-ttu-id="f8931-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8931-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8931-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8931-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8931-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8931-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8931-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f8931-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8931-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8931-108">Prerequisites</span></span>
<span data-ttu-id="f8931-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8931-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8931-111">Permission type</span></span>|<span data-ttu-id="f8931-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8931-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8931-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8931-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8931-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8931-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8931-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8931-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8931-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8931-116">Not supported.</span></span>|
|<span data-ttu-id="f8931-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8931-117">Application</span></span>|<span data-ttu-id="f8931-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8931-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8931-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8931-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f8931-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8931-120">Request headers</span></span>
|<span data-ttu-id="f8931-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8931-121">Header</span></span>|<span data-ttu-id="f8931-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8931-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8931-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8931-123">Authorization</span></span>|<span data-ttu-id="f8931-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8931-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8931-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8931-125">Accept</span></span>|<span data-ttu-id="f8931-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8931-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8931-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8931-127">Request body</span></span>
<span data-ttu-id="f8931-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f8931-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f8931-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f8931-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f8931-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8931-130">Property</span></span>|<span data-ttu-id="f8931-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8931-131">Type</span></span>|<span data-ttu-id="f8931-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8931-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8931-133">assignments</span><span class="sxs-lookup"><span data-stu-id="f8931-133">assignments</span></span>|<span data-ttu-id="f8931-134">[Coleção deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f8931-134">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="f8931-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f8931-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f8931-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8931-136">Response</span></span>
<span data-ttu-id="f8931-137">Se tiver êxito, esta ação retornará um código de resposta e uma coleção `200 OK` [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8931-137">If successful, this action returns a `200 OK` response code and a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8931-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8931-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8931-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8931-139">Request</span></span>
<span data-ttu-id="f8931-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8931-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8931-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8931-141">Response</span></span>
<span data-ttu-id="f8931-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8931-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




