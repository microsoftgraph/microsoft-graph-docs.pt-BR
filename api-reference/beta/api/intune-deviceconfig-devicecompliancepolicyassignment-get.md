---
title: Acessar deviceCompliancePolicyAssignment
description: Leia as propriedades e as relações do objeto deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f315fd7a5677b247b74cae796247246dc7f0db2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155474"
---
# <a name="get-devicecompliancepolicyassignment"></a><span data-ttu-id="de1b3-103">Acessar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="de1b3-103">Get deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="de1b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de1b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de1b3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de1b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de1b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de1b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de1b3-107">Leia as propriedades e as relações do objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de1b3-107">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de1b3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de1b3-108">Prerequisites</span></span>
<span data-ttu-id="de1b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de1b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de1b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de1b3-111">Permission type</span></span>|<span data-ttu-id="de1b3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de1b3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de1b3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de1b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de1b3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de1b3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de1b3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de1b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de1b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de1b3-116">Not supported.</span></span>|
|<span data-ttu-id="de1b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de1b3-117">Application</span></span>|<span data-ttu-id="de1b3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de1b3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de1b3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de1b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de1b3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de1b3-120">Optional query parameters</span></span>
<span data-ttu-id="de1b3-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de1b3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de1b3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de1b3-122">Request headers</span></span>
|<span data-ttu-id="de1b3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de1b3-123">Header</span></span>|<span data-ttu-id="de1b3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="de1b3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de1b3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="de1b3-125">Authorization</span></span>|<span data-ttu-id="de1b3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de1b3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de1b3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de1b3-127">Accept</span></span>|<span data-ttu-id="de1b3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="de1b3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de1b3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de1b3-129">Request body</span></span>
<span data-ttu-id="de1b3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de1b3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de1b3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="de1b3-131">Response</span></span>
<span data-ttu-id="de1b3-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de1b3-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de1b3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de1b3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="de1b3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de1b3-134">Request</span></span>
<span data-ttu-id="de1b3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de1b3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="de1b3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="de1b3-136">Response</span></span>
<span data-ttu-id="de1b3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de1b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 540

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
    "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
    "target": {
      "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include",
      "collectionId": "Collection Id value"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```




