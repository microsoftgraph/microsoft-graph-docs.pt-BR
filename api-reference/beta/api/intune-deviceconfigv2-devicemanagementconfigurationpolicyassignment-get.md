---
title: Obter deviceManagementConfigurationPolicyAssignment
description: Leia as propriedades e as relações do objeto deviceManagementConfigurationPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0a8c314f7925ce50b440b203b0b6c5e96038a47
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301461"
---
# <a name="get-devicemanagementconfigurationpolicyassignment"></a><span data-ttu-id="d5bff-103">Obter deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d5bff-103">Get deviceManagementConfigurationPolicyAssignment</span></span>

<span data-ttu-id="d5bff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5bff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5bff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5bff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5bff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5bff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5bff-107">Leia as propriedades e as relações do objeto [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d5bff-107">Read properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5bff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5bff-108">Prerequisites</span></span>
<span data-ttu-id="d5bff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5bff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5bff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5bff-111">Permission type</span></span>|<span data-ttu-id="d5bff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5bff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5bff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5bff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5bff-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5bff-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d5bff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5bff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5bff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bff-116">Not supported.</span></span>|
|<span data-ttu-id="d5bff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5bff-117">Application</span></span>|<span data-ttu-id="d5bff-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5bff-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5bff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5bff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5bff-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d5bff-120">Optional query parameters</span></span>
<span data-ttu-id="d5bff-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5bff-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5bff-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bff-122">Request headers</span></span>
|<span data-ttu-id="d5bff-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5bff-123">Header</span></span>|<span data-ttu-id="d5bff-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d5bff-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5bff-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5bff-125">Authorization</span></span>|<span data-ttu-id="d5bff-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5bff-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5bff-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5bff-127">Accept</span></span>|<span data-ttu-id="d5bff-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d5bff-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5bff-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bff-129">Request body</span></span>
<span data-ttu-id="d5bff-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5bff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5bff-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bff-131">Response</span></span>
<span data-ttu-id="d5bff-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5bff-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5bff-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5bff-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5bff-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bff-134">Request</span></span>
<span data-ttu-id="d5bff-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5bff-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/assignments/{deviceManagementConfigurationPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d5bff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bff-136">Response</span></span>
<span data-ttu-id="d5bff-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5bff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
    "id": "1f069921-9921-1f06-2199-061f2199061f",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```




