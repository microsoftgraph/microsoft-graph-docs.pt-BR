---
title: Obter deviceManagementIntentAssignment
description: Leia as propriedades e as relações do objeto deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b18f216358c7aba6e214cc54288f1dc918b2ae9c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229734"
---
# <a name="get-devicemanagementintentassignment"></a><span data-ttu-id="6e0f6-103">Obter deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="6e0f6-103">Get deviceManagementIntentAssignment</span></span>

<span data-ttu-id="6e0f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e0f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e0f6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e0f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e0f6-107">Leia as propriedades e as relações do objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6e0f6-107">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e0f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e0f6-108">Prerequisites</span></span>
<span data-ttu-id="6e0f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e0f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e0f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e0f6-111">Permission type</span></span>|<span data-ttu-id="6e0f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e0f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e0f6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e0f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e0f6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e0f6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6e0f6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e0f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e0f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-116">Not supported.</span></span>|
|<span data-ttu-id="6e0f6-117">Application</span><span class="sxs-lookup"><span data-stu-id="6e0f6-117">Application</span></span>|<span data-ttu-id="6e0f6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e0f6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e0f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e0f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e0f6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e0f6-120">Optional query parameters</span></span>
<span data-ttu-id="6e0f6-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e0f6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e0f6-122">Request headers</span></span>
|<span data-ttu-id="6e0f6-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e0f6-123">Header</span></span>|<span data-ttu-id="6e0f6-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6e0f6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e0f6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e0f6-125">Authorization</span></span>|<span data-ttu-id="6e0f6-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e0f6-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e0f6-127">Accept</span></span>|<span data-ttu-id="6e0f6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6e0f6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e0f6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e0f6-129">Request body</span></span>
<span data-ttu-id="6e0f6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e0f6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e0f6-131">Response</span></span>
<span data-ttu-id="6e0f6-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e0f6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e0f6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e0f6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e0f6-134">Request</span></span>
<span data-ttu-id="6e0f6-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6e0f6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e0f6-136">Response</span></span>
<span data-ttu-id="6e0f6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e0f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
    "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```




