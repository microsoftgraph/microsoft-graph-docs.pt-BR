---
title: Listar deviceAppManagementTasks
description: Listar propriedades e relações dos objetos deviceAppManagementTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e281fcad7e005855b5c83393fc61e173260bdb5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134883"
---
# <a name="list-deviceappmanagementtasks"></a><span data-ttu-id="4068b-103">Listar deviceAppManagementTasks</span><span class="sxs-lookup"><span data-stu-id="4068b-103">List deviceAppManagementTasks</span></span>

<span data-ttu-id="4068b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4068b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4068b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4068b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4068b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4068b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4068b-107">Listar propriedades e relações dos [objetos deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="4068b-107">List properties and relationships of the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4068b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4068b-108">Prerequisites</span></span>
<span data-ttu-id="4068b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4068b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4068b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4068b-111">Permission type</span></span>|<span data-ttu-id="4068b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4068b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4068b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4068b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4068b-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4068b-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4068b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4068b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4068b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4068b-116">Not supported.</span></span>|
|<span data-ttu-id="4068b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4068b-117">Application</span></span>|<span data-ttu-id="4068b-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4068b-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4068b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4068b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="4068b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4068b-120">Request headers</span></span>
|<span data-ttu-id="4068b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4068b-121">Header</span></span>|<span data-ttu-id="4068b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4068b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4068b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4068b-123">Authorization</span></span>|<span data-ttu-id="4068b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4068b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4068b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4068b-125">Accept</span></span>|<span data-ttu-id="4068b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4068b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4068b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4068b-127">Request body</span></span>
<span data-ttu-id="4068b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4068b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4068b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4068b-129">Response</span></span>
<span data-ttu-id="4068b-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4068b-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4068b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4068b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4068b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4068b-132">Request</span></span>
<span data-ttu-id="4068b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4068b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### <a name="response"></a><span data-ttu-id="4068b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4068b-134">Response</span></span>
<span data-ttu-id="4068b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4068b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




