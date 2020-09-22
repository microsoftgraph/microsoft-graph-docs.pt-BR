---
title: Listar deviceManagementIntentAssignments
description: Listar Propriedades e relações dos objetos deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b68aa9d142a30929340d0ac375da4d866200bd37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994733"
---
# <a name="list-devicemanagementintentassignments"></a><span data-ttu-id="1ed67-103">Listar deviceManagementIntentAssignments</span><span class="sxs-lookup"><span data-stu-id="1ed67-103">List deviceManagementIntentAssignments</span></span>

<span data-ttu-id="1ed67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ed67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ed67-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ed67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ed67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ed67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ed67-107">Listar Propriedades e relações dos objetos [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1ed67-107">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ed67-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ed67-108">Prerequisites</span></span>
<span data-ttu-id="1ed67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ed67-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ed67-111">Permission type</span></span>|<span data-ttu-id="1ed67-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ed67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ed67-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ed67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ed67-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ed67-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ed67-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ed67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ed67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ed67-116">Not supported.</span></span>|
|<span data-ttu-id="1ed67-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ed67-117">Application</span></span>|<span data-ttu-id="1ed67-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ed67-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ed67-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ed67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1ed67-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed67-120">Request headers</span></span>
|<span data-ttu-id="1ed67-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ed67-121">Header</span></span>|<span data-ttu-id="1ed67-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1ed67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ed67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ed67-123">Authorization</span></span>|<span data-ttu-id="1ed67-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ed67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ed67-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ed67-125">Accept</span></span>|<span data-ttu-id="1ed67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ed67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ed67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed67-127">Request body</span></span>
<span data-ttu-id="1ed67-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ed67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ed67-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ed67-129">Response</span></span>
<span data-ttu-id="1ed67-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ed67-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ed67-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ed67-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ed67-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed67-132">Request</span></span>
<span data-ttu-id="1ed67-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ed67-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments
```

### <a name="response"></a><span data-ttu-id="1ed67-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ed67-134">Response</span></span>
<span data-ttu-id="1ed67-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ed67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 437

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
      "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```






