---
title: Listar securityConfigurationTasks
description: Listar Propriedades e relações dos objetos securityConfigurationTask.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3f732c5aeb5b7b2876ce9e96129bc606804b44c
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793150"
---
# <a name="list-securityconfigurationtasks"></a><span data-ttu-id="ee972-103">Listar securityConfigurationTasks</span><span class="sxs-lookup"><span data-stu-id="ee972-103">List securityConfigurationTasks</span></span>

<span data-ttu-id="ee972-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee972-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee972-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee972-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee972-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee972-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee972-107">Listar Propriedades e relações dos objetos [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) .</span><span class="sxs-lookup"><span data-stu-id="ee972-107">List properties and relationships of the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee972-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee972-108">Prerequisites</span></span>
<span data-ttu-id="ee972-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee972-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee972-111">Permission type</span></span>|<span data-ttu-id="ee972-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee972-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee972-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee972-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee972-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee972-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ee972-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee972-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee972-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee972-116">Not supported.</span></span>|
|<span data-ttu-id="ee972-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee972-117">Application</span></span>|<span data-ttu-id="ee972-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee972-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee972-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee972-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="ee972-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee972-120">Request headers</span></span>
|<span data-ttu-id="ee972-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee972-121">Header</span></span>|<span data-ttu-id="ee972-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee972-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee972-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee972-123">Authorization</span></span>|<span data-ttu-id="ee972-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee972-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee972-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee972-125">Accept</span></span>|<span data-ttu-id="ee972-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee972-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee972-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee972-127">Request body</span></span>
<span data-ttu-id="ee972-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee972-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee972-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee972-129">Response</span></span>
<span data-ttu-id="ee972-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee972-130">If successful, this method returns a `200 OK` response code and a collection of [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee972-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee972-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee972-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee972-132">Request</span></span>
<span data-ttu-id="ee972-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee972-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### <a name="response"></a><span data-ttu-id="ee972-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee972-134">Response</span></span>
<span data-ttu-id="ee972-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee972-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 983

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityConfigurationTask",
      "id": "5d630f12-0f12-5d63-120f-635d120f635d",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
      "category": "advancedThreatProtection",
      "priority": "high",
      "creator": "Creator value",
      "creatorNotes": "Creator Notes value",
      "assignedTo": "Assigned To value",
      "status": "pending",
      "endpointSecurityPolicy": "antivirus",
      "applicablePlatform": "macOS",
      "endpointSecurityPolicyProfile": "antivirus",
      "insights": "Insights value",
      "managedDeviceCount": 2,
      "intendedSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```



