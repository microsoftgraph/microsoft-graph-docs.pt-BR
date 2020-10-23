---
title: Listar locationManagementConditions
description: Listar Propriedades e relações dos objetos locationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47ca6395a4740f9859f63c9b4ab762f05d260a6e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701939"
---
# <a name="list-locationmanagementconditions"></a><span data-ttu-id="6bfa4-103">Listar locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="6bfa4-103">List locationManagementConditions</span></span>

<span data-ttu-id="6bfa4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bfa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bfa4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bfa4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bfa4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bfa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bfa4-107">Listar Propriedades e relações dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="6bfa4-107">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bfa4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bfa4-108">Prerequisites</span></span>
<span data-ttu-id="6bfa4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bfa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bfa4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bfa4-111">Permission type</span></span>|<span data-ttu-id="6bfa4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bfa4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bfa4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bfa4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bfa4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bfa4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6bfa4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bfa4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bfa4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bfa4-116">Not supported.</span></span>|
|<span data-ttu-id="6bfa4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bfa4-117">Application</span></span>|<span data-ttu-id="6bfa4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bfa4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bfa4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bfa4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="6bfa4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfa4-120">Request headers</span></span>
|<span data-ttu-id="6bfa4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bfa4-121">Header</span></span>|<span data-ttu-id="6bfa4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6bfa4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bfa4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bfa4-123">Authorization</span></span>|<span data-ttu-id="6bfa4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bfa4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bfa4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bfa4-125">Accept</span></span>|<span data-ttu-id="6bfa4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bfa4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bfa4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfa4-127">Request body</span></span>
<span data-ttu-id="6bfa4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6bfa4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bfa4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bfa4-129">Response</span></span>
<span data-ttu-id="6bfa4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bfa4-130">If successful, this method returns a `200 OK` response code and a collection of [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bfa4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bfa4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bfa4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bfa4-132">Request</span></span>
<span data-ttu-id="6bfa4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bfa4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="6bfa4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bfa4-134">Response</span></span>
<span data-ttu-id="6bfa4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bfa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.locationManagementCondition",
      "id": "23b1ca32-ca32-23b1-32ca-b12332cab123",
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





