---
title: Lista deviceManagementScriptGroupAssignments
description: Lista as propriedades e os relacionamentos dos objetos deviceManagementScriptGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b760d39bd6d836feeb6f89f52bc9e96e0f945b9c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392819"
---
# <a name="list-devicemanagementscriptgroupassignments"></a><span data-ttu-id="d8141-103">Lista deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="d8141-103">List deviceManagementScriptGroupAssignments</span></span>

> <span data-ttu-id="d8141-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8141-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8141-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8141-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8141-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d8141-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8141-107">Lista as propriedades e os relacionamentos dos objetos [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d8141-107">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8141-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8141-108">Prerequisites</span></span>
<span data-ttu-id="d8141-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8141-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8141-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8141-111">Permission type</span></span>|<span data-ttu-id="d8141-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8141-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8141-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8141-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8141-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8141-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d8141-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8141-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8141-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8141-116">Not supported.</span></span>|
|<span data-ttu-id="d8141-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8141-117">Application</span></span>|<span data-ttu-id="d8141-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8141-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8141-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8141-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="d8141-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8141-120">Request headers</span></span>
|<span data-ttu-id="d8141-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8141-121">Header</span></span>|<span data-ttu-id="d8141-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8141-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8141-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8141-123">Authorization</span></span>|<span data-ttu-id="d8141-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8141-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8141-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8141-125">Accept</span></span>|<span data-ttu-id="d8141-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8141-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8141-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8141-127">Request body</span></span>
<span data-ttu-id="d8141-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8141-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8141-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8141-129">Response</span></span>
<span data-ttu-id="d8141-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8141-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8141-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8141-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8141-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8141-132">Request</span></span>
<span data-ttu-id="d8141-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8141-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="d8141-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8141-134">Response</span></span>
<span data-ttu-id="d8141-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8141-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```




