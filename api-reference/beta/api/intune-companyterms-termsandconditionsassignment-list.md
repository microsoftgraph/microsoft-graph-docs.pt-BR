---
title: Listar termsAndConditionsAssignments
description: Listar propriedades e relações dos objetos termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67624a0e1f20a730a25e4f61f4f6261cc7231118
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793161"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="1a6d0-103">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="1a6d0-103">List termsAndConditionsAssignments</span></span>

<span data-ttu-id="1a6d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a6d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a6d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a6d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a6d0-107">Listar propriedades e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1a6d0-107">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a6d0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a6d0-108">Prerequisites</span></span>
<span data-ttu-id="1a6d0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1a6d0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a6d0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a6d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a6d0-111">Permission type</span></span>|<span data-ttu-id="1a6d0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a6d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a6d0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a6d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a6d0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a6d0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1a6d0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a6d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a6d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-116">Not supported.</span></span>|
|<span data-ttu-id="1a6d0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a6d0-117">Application</span></span>|<span data-ttu-id="1a6d0-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a6d0-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a6d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a6d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1a6d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a6d0-120">Request headers</span></span>
|<span data-ttu-id="1a6d0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a6d0-121">Header</span></span>|<span data-ttu-id="1a6d0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1a6d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a6d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a6d0-123">Authorization</span></span>|<span data-ttu-id="1a6d0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a6d0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a6d0-125">Accept</span></span>|<span data-ttu-id="1a6d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a6d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a6d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a6d0-127">Request body</span></span>
<span data-ttu-id="1a6d0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a6d0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a6d0-129">Response</span></span>
<span data-ttu-id="1a6d0-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a6d0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a6d0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a6d0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a6d0-132">Request</span></span>
<span data-ttu-id="1a6d0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="1a6d0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a6d0-134">Response</span></span>
<span data-ttu-id="1a6d0-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-135">Here is an example of the response.</span></span> <span data-ttu-id="1a6d0-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1a6d0-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1a6d0-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



