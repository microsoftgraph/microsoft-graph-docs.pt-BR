---
title: Atualizar deviceManagementIntentUserStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentUserStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1661770f444fe7479d47858ce6e8ad394d3ed98e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805709"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="437c8-103">Atualizar deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="437c8-103">Update deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="437c8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="437c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="437c8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="437c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="437c8-106">Atualiza as propriedades de um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="437c8-106">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="437c8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="437c8-107">Prerequisites</span></span>
<span data-ttu-id="437c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="437c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="437c8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="437c8-110">Permission type</span></span>|<span data-ttu-id="437c8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="437c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="437c8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="437c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="437c8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="437c8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="437c8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="437c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="437c8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="437c8-115">Not supported.</span></span>|
|<span data-ttu-id="437c8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="437c8-116">Application</span></span>|<span data-ttu-id="437c8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="437c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="437c8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="437c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="437c8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="437c8-119">Request headers</span></span>
|<span data-ttu-id="437c8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="437c8-120">Header</span></span>|<span data-ttu-id="437c8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="437c8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="437c8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="437c8-122">Authorization</span></span>|<span data-ttu-id="437c8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="437c8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="437c8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="437c8-124">Accept</span></span>|<span data-ttu-id="437c8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="437c8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="437c8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="437c8-126">Request body</span></span>
<span data-ttu-id="437c8-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="437c8-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="437c8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="437c8-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="437c8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="437c8-129">Property</span></span>|<span data-ttu-id="437c8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="437c8-130">Type</span></span>|<span data-ttu-id="437c8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="437c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="437c8-132">id</span><span class="sxs-lookup"><span data-stu-id="437c8-132">id</span></span>|<span data-ttu-id="437c8-133">String</span><span class="sxs-lookup"><span data-stu-id="437c8-133">String</span></span>|<span data-ttu-id="437c8-134">A ID</span><span class="sxs-lookup"><span data-stu-id="437c8-134">The ID</span></span>|
|<span data-ttu-id="437c8-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="437c8-135">conflictCount</span></span>|<span data-ttu-id="437c8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="437c8-136">Int32</span></span>|<span data-ttu-id="437c8-137">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="437c8-137">Number of users in conflict</span></span>|
|<span data-ttu-id="437c8-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="437c8-138">errorCount</span></span>|<span data-ttu-id="437c8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="437c8-139">Int32</span></span>|<span data-ttu-id="437c8-140">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="437c8-140">Number of error users</span></span>|
|<span data-ttu-id="437c8-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="437c8-141">failedCount</span></span>|<span data-ttu-id="437c8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="437c8-142">Int32</span></span>|<span data-ttu-id="437c8-143">Número de usuários com falha</span><span class="sxs-lookup"><span data-stu-id="437c8-143">Number of failed users</span></span>|
|<span data-ttu-id="437c8-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="437c8-144">notApplicableCount</span></span>|<span data-ttu-id="437c8-145">Int32</span><span class="sxs-lookup"><span data-stu-id="437c8-145">Int32</span></span>|<span data-ttu-id="437c8-146">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="437c8-146">Number of not applicable users</span></span>|
|<span data-ttu-id="437c8-147">successCount</span><span class="sxs-lookup"><span data-stu-id="437c8-147">successCount</span></span>|<span data-ttu-id="437c8-148">Int32</span><span class="sxs-lookup"><span data-stu-id="437c8-148">Int32</span></span>|<span data-ttu-id="437c8-149">Número de usuários com êxito</span><span class="sxs-lookup"><span data-stu-id="437c8-149">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="437c8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="437c8-150">Response</span></span>
<span data-ttu-id="437c8-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="437c8-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="437c8-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="437c8-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="437c8-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="437c8-153">Request</span></span>
<span data-ttu-id="437c8-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="437c8-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="437c8-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="437c8-155">Response</span></span>
<span data-ttu-id="437c8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="437c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





