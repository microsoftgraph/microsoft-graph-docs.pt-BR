---
title: Listar deviceAppManagementTasks
description: Listar Propriedades e relações dos objetos deviceAppManagementTask.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e446ec95071e6760123a09c668a0355ae9e39789
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445332"
---
# <a name="list-deviceappmanagementtasks"></a><span data-ttu-id="e87bb-103">Listar deviceAppManagementTasks</span><span class="sxs-lookup"><span data-stu-id="e87bb-103">List deviceAppManagementTasks</span></span>

<span data-ttu-id="e87bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e87bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e87bb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e87bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e87bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e87bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e87bb-107">Listar Propriedades e relações dos objetos [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) .</span><span class="sxs-lookup"><span data-stu-id="e87bb-107">List properties and relationships of the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e87bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e87bb-108">Prerequisites</span></span>
<span data-ttu-id="e87bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e87bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e87bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e87bb-111">Permission type</span></span>|<span data-ttu-id="e87bb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e87bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e87bb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e87bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e87bb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e87bb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e87bb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e87bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e87bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e87bb-116">Not supported.</span></span>|
|<span data-ttu-id="e87bb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e87bb-117">Application</span></span>|<span data-ttu-id="e87bb-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e87bb-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e87bb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e87bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="e87bb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e87bb-120">Request headers</span></span>
|<span data-ttu-id="e87bb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e87bb-121">Header</span></span>|<span data-ttu-id="e87bb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e87bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e87bb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e87bb-123">Authorization</span></span>|<span data-ttu-id="e87bb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e87bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e87bb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e87bb-125">Accept</span></span>|<span data-ttu-id="e87bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e87bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e87bb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e87bb-127">Request body</span></span>
<span data-ttu-id="e87bb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e87bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e87bb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e87bb-129">Response</span></span>
<span data-ttu-id="e87bb-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e87bb-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e87bb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e87bb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e87bb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e87bb-132">Request</span></span>
<span data-ttu-id="e87bb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e87bb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### <a name="response"></a><span data-ttu-id="e87bb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e87bb-134">Response</span></span>
<span data-ttu-id="e87bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e87bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 589

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAppManagementTask",
      "id": "814545cc-45cc-8145-cc45-4581cc454581",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
      "category": "advancedThreatProtection",
      "priority": "high",
      "creator": "Creator value",
      "creatorNotes": "Creator Notes value",
      "assignedTo": "Assigned To value",
      "status": "pending"
    }
  ]
}
```



