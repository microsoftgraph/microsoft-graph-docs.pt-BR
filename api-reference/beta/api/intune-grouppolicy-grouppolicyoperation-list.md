---
title: Listar groupPolicyOperations
description: Listar Propriedades e relações dos objetos groupPolicyOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9477538e4ea62419a82c4f0fd4b6e2b1d98bc009
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078826"
---
# <a name="list-grouppolicyoperations"></a><span data-ttu-id="bb504-103">Listar groupPolicyOperations</span><span class="sxs-lookup"><span data-stu-id="bb504-103">List groupPolicyOperations</span></span>

<span data-ttu-id="bb504-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb504-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb504-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb504-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb504-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb504-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb504-107">Listar Propriedades e relações dos objetos [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="bb504-107">List properties and relationships of the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb504-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb504-108">Prerequisites</span></span>
<span data-ttu-id="bb504-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb504-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb504-111">Permission type</span></span>|<span data-ttu-id="bb504-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb504-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb504-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb504-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb504-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb504-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bb504-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb504-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb504-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb504-116">Not supported.</span></span>|
|<span data-ttu-id="bb504-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb504-117">Application</span></span>|<span data-ttu-id="bb504-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb504-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb504-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb504-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
```

## <a name="request-headers"></a><span data-ttu-id="bb504-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb504-120">Request headers</span></span>
|<span data-ttu-id="bb504-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb504-121">Header</span></span>|<span data-ttu-id="bb504-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bb504-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb504-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb504-123">Authorization</span></span>|<span data-ttu-id="bb504-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb504-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb504-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb504-125">Accept</span></span>|<span data-ttu-id="bb504-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb504-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb504-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb504-127">Request body</span></span>
<span data-ttu-id="bb504-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb504-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb504-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb504-129">Response</span></span>
<span data-ttu-id="bb504-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb504-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb504-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb504-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb504-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb504-132">Request</span></span>
<span data-ttu-id="bb504-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb504-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
```

### <a name="response"></a><span data-ttu-id="bb504-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb504-134">Response</span></span>
<span data-ttu-id="bb504-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb504-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyOperation",
      "operationType": "upload",
      "operationStatus": "inProgress",
      "statusDetails": "Status Details value",
      "id": "4d18865b-865b-4d18-5b86-184d5b86184d",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```






