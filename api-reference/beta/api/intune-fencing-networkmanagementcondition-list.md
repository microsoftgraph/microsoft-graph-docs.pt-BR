---
title: Listar networkManagementConditions
description: Listar propriedades e relações dos objetos networkManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 282f5ee0494778897f50f4b4c3c341d60c448e15
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142055"
---
# <a name="list-networkmanagementconditions"></a><span data-ttu-id="e3df6-103">Listar networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="e3df6-103">List networkManagementConditions</span></span>

<span data-ttu-id="e3df6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3df6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3df6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3df6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3df6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3df6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3df6-107">Listar propriedades e relações dos objetos [networkManagementCondition.](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e3df6-107">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3df6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3df6-108">Prerequisites</span></span>
<span data-ttu-id="e3df6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3df6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3df6-111">Permission type</span></span>|<span data-ttu-id="e3df6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3df6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3df6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3df6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3df6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3df6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3df6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3df6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3df6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3df6-116">Not supported.</span></span>|
|<span data-ttu-id="e3df6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3df6-117">Application</span></span>|<span data-ttu-id="e3df6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3df6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3df6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3df6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="e3df6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3df6-120">Request headers</span></span>
|<span data-ttu-id="e3df6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3df6-121">Header</span></span>|<span data-ttu-id="e3df6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e3df6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3df6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3df6-123">Authorization</span></span>|<span data-ttu-id="e3df6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3df6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3df6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3df6-125">Accept</span></span>|<span data-ttu-id="e3df6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3df6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3df6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3df6-127">Request body</span></span>
<span data-ttu-id="e3df6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3df6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3df6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3df6-129">Response</span></span>
<span data-ttu-id="e3df6-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3df6-130">If successful, this method returns a `200 OK` response code and a collection of [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3df6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3df6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3df6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3df6-132">Request</span></span>
<span data-ttu-id="e3df6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3df6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="e3df6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3df6-134">Response</span></span>
<span data-ttu-id="e3df6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3df6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkManagementCondition",
      "id": "c2919b8f-9b8f-c291-8f9b-91c28f9b91c2",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```




