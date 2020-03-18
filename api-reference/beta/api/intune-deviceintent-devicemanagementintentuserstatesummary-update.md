---
title: Atualizar deviceManagementIntentUserStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentUserStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88749a89e92ffa3069c929b4e754627049491725
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765808"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="e22b9-103">Atualizar deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="e22b9-103">Update deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="e22b9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e22b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e22b9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e22b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e22b9-106">Atualiza as propriedades de um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e22b9-106">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e22b9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e22b9-107">Prerequisites</span></span>
<span data-ttu-id="e22b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e22b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e22b9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e22b9-110">Permission type</span></span>|<span data-ttu-id="e22b9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e22b9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e22b9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e22b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e22b9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22b9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e22b9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e22b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e22b9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e22b9-115">Not supported.</span></span>|
|<span data-ttu-id="e22b9-116">Application</span><span class="sxs-lookup"><span data-stu-id="e22b9-116">Application</span></span>|<span data-ttu-id="e22b9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22b9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e22b9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e22b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="e22b9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e22b9-119">Request headers</span></span>
|<span data-ttu-id="e22b9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e22b9-120">Header</span></span>|<span data-ttu-id="e22b9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e22b9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e22b9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e22b9-122">Authorization</span></span>|<span data-ttu-id="e22b9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e22b9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e22b9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e22b9-124">Accept</span></span>|<span data-ttu-id="e22b9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e22b9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e22b9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e22b9-126">Request body</span></span>
<span data-ttu-id="e22b9-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e22b9-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="e22b9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e22b9-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="e22b9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e22b9-129">Property</span></span>|<span data-ttu-id="e22b9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e22b9-130">Type</span></span>|<span data-ttu-id="e22b9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e22b9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e22b9-132">id</span><span class="sxs-lookup"><span data-stu-id="e22b9-132">id</span></span>|<span data-ttu-id="e22b9-133">String</span><span class="sxs-lookup"><span data-stu-id="e22b9-133">String</span></span>|<span data-ttu-id="e22b9-134">A ID</span><span class="sxs-lookup"><span data-stu-id="e22b9-134">The ID</span></span>|
|<span data-ttu-id="e22b9-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e22b9-135">conflictCount</span></span>|<span data-ttu-id="e22b9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e22b9-136">Int32</span></span>|<span data-ttu-id="e22b9-137">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="e22b9-137">Number of users in conflict</span></span>|
|<span data-ttu-id="e22b9-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="e22b9-138">errorCount</span></span>|<span data-ttu-id="e22b9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e22b9-139">Int32</span></span>|<span data-ttu-id="e22b9-140">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="e22b9-140">Number of error users</span></span>|
|<span data-ttu-id="e22b9-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="e22b9-141">failedCount</span></span>|<span data-ttu-id="e22b9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e22b9-142">Int32</span></span>|<span data-ttu-id="e22b9-143">Número de usuários com falha</span><span class="sxs-lookup"><span data-stu-id="e22b9-143">Number of failed users</span></span>|
|<span data-ttu-id="e22b9-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e22b9-144">notApplicableCount</span></span>|<span data-ttu-id="e22b9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e22b9-145">Int32</span></span>|<span data-ttu-id="e22b9-146">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="e22b9-146">Number of not applicable users</span></span>|
|<span data-ttu-id="e22b9-147">successCount</span><span class="sxs-lookup"><span data-stu-id="e22b9-147">successCount</span></span>|<span data-ttu-id="e22b9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e22b9-148">Int32</span></span>|<span data-ttu-id="e22b9-149">Número de usuários com êxito</span><span class="sxs-lookup"><span data-stu-id="e22b9-149">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="e22b9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e22b9-150">Response</span></span>
<span data-ttu-id="e22b9-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e22b9-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e22b9-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e22b9-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e22b9-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e22b9-153">Request</span></span>
<span data-ttu-id="e22b9-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e22b9-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
Content-type: application/json
Content-length: 198

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```

### <a name="response"></a><span data-ttu-id="e22b9-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e22b9-155">Response</span></span>
<span data-ttu-id="e22b9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e22b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "be567e02-7e02-be56-027e-56be027e56be",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```




