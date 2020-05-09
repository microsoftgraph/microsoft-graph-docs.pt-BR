---
title: Atualizar deviceManagementIntentAssignment
description: Atualiza as propriedades de um objeto deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d6feeba8e0c2fd332efc68a18e4d4976068394b
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177216"
---
# <a name="update-devicemanagementintentassignment"></a><span data-ttu-id="01ca3-103">Atualizar deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="01ca3-103">Update deviceManagementIntentAssignment</span></span>

<span data-ttu-id="01ca3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01ca3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01ca3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01ca3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01ca3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01ca3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01ca3-107">Atualiza as propriedades de um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="01ca3-107">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01ca3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01ca3-108">Prerequisites</span></span>
<span data-ttu-id="01ca3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01ca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01ca3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01ca3-111">Permission type</span></span>|<span data-ttu-id="01ca3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01ca3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01ca3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01ca3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01ca3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01ca3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01ca3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01ca3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01ca3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01ca3-116">Not supported.</span></span>|
|<span data-ttu-id="01ca3-117">Application</span><span class="sxs-lookup"><span data-stu-id="01ca3-117">Application</span></span>|<span data-ttu-id="01ca3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01ca3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01ca3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01ca3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="01ca3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01ca3-120">Request headers</span></span>
|<span data-ttu-id="01ca3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01ca3-121">Header</span></span>|<span data-ttu-id="01ca3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01ca3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01ca3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01ca3-123">Authorization</span></span>|<span data-ttu-id="01ca3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01ca3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01ca3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01ca3-125">Accept</span></span>|<span data-ttu-id="01ca3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01ca3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01ca3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01ca3-127">Request body</span></span>
<span data-ttu-id="01ca3-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="01ca3-128">In the request body, supply a JSON representation for the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

<span data-ttu-id="01ca3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span><span class="sxs-lookup"><span data-stu-id="01ca3-129">The following table shows the properties that are required when you create the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>

|<span data-ttu-id="01ca3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01ca3-130">Property</span></span>|<span data-ttu-id="01ca3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01ca3-131">Type</span></span>|<span data-ttu-id="01ca3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01ca3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01ca3-133">id</span><span class="sxs-lookup"><span data-stu-id="01ca3-133">id</span></span>|<span data-ttu-id="01ca3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01ca3-134">String</span></span>|<span data-ttu-id="01ca3-135">A ID da atribuição</span><span class="sxs-lookup"><span data-stu-id="01ca3-135">The assignment ID</span></span>|
|<span data-ttu-id="01ca3-136">destino</span><span class="sxs-lookup"><span data-stu-id="01ca3-136">target</span></span>|[<span data-ttu-id="01ca3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="01ca3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="01ca3-138">O destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="01ca3-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="01ca3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="01ca3-139">Response</span></span>
<span data-ttu-id="01ca3-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01ca3-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01ca3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01ca3-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="01ca3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01ca3-142">Request</span></span>
<span data-ttu-id="01ca3-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01ca3-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
Content-type: application/json
Content-length: 160

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="01ca3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="01ca3-144">Response</span></span>
<span data-ttu-id="01ca3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01ca3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



