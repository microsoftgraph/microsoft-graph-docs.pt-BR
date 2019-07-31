---
title: Listar groupPolicyConfigurationAssignments
description: Listar Propriedades e relações dos objetos groupPolicyConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99908580a770ba65eb17676e7610d2f6f1adb67a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989977"
---
# <a name="list-grouppolicyconfigurationassignments"></a><span data-ttu-id="13a1a-103">Listar groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="13a1a-103">List groupPolicyConfigurationAssignments</span></span>

> <span data-ttu-id="13a1a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13a1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13a1a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13a1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13a1a-106">Listar Propriedades e relações dos objetos [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="13a1a-106">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13a1a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13a1a-107">Prerequisites</span></span>
<span data-ttu-id="13a1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13a1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13a1a-110">Permission type</span></span>|<span data-ttu-id="13a1a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="13a1a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13a1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13a1a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13a1a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="13a1a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="13a1a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13a1a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13a1a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13a1a-115">Not supported.</span></span>|
|<span data-ttu-id="13a1a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13a1a-116">Application</span></span>|<span data-ttu-id="13a1a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13a1a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13a1a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13a1a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="13a1a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13a1a-119">Request headers</span></span>
|<span data-ttu-id="13a1a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13a1a-120">Header</span></span>|<span data-ttu-id="13a1a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="13a1a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13a1a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13a1a-122">Authorization</span></span>|<span data-ttu-id="13a1a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13a1a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13a1a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="13a1a-124">Accept</span></span>|<span data-ttu-id="13a1a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13a1a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13a1a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13a1a-126">Request body</span></span>
<span data-ttu-id="13a1a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13a1a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13a1a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="13a1a-128">Response</span></span>
<span data-ttu-id="13a1a-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13a1a-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a1a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13a1a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="13a1a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13a1a-131">Request</span></span>
<span data-ttu-id="13a1a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13a1a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="13a1a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="13a1a-133">Response</span></span>
<span data-ttu-id="13a1a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13a1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





