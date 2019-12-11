---
title: Atualizar deviceManagementIntentUserStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentUserStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfed353edb085af7acb32fc7019918abb8e06591
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945631"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="8e3f5-103">Atualizar deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="8e3f5-103">Update deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="8e3f5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e3f5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e3f5-106">Atualiza as propriedades de um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="8e3f5-106">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e3f5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e3f5-107">Prerequisites</span></span>
<span data-ttu-id="8e3f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e3f5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e3f5-110">Permission type</span></span>|<span data-ttu-id="8e3f5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e3f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e3f5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e3f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e3f5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e3f5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e3f5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e3f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e3f5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-115">Not supported.</span></span>|
|<span data-ttu-id="8e3f5-116">Application</span><span class="sxs-lookup"><span data-stu-id="8e3f5-116">Application</span></span>|<span data-ttu-id="8e3f5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e3f5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e3f5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e3f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="8e3f5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3f5-119">Request headers</span></span>
|<span data-ttu-id="8e3f5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e3f5-120">Header</span></span>|<span data-ttu-id="8e3f5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e3f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e3f5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e3f5-122">Authorization</span></span>|<span data-ttu-id="8e3f5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e3f5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e3f5-124">Accept</span></span>|<span data-ttu-id="8e3f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e3f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e3f5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3f5-126">Request body</span></span>
<span data-ttu-id="8e3f5-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="8e3f5-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="8e3f5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8e3f5-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="8e3f5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e3f5-129">Property</span></span>|<span data-ttu-id="8e3f5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e3f5-130">Type</span></span>|<span data-ttu-id="8e3f5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e3f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e3f5-132">id</span><span class="sxs-lookup"><span data-stu-id="8e3f5-132">id</span></span>|<span data-ttu-id="8e3f5-133">String</span><span class="sxs-lookup"><span data-stu-id="8e3f5-133">String</span></span>|<span data-ttu-id="8e3f5-134">A ID</span><span class="sxs-lookup"><span data-stu-id="8e3f5-134">The ID</span></span>|
|<span data-ttu-id="8e3f5-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="8e3f5-135">conflictCount</span></span>|<span data-ttu-id="8e3f5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3f5-136">Int32</span></span>|<span data-ttu-id="8e3f5-137">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="8e3f5-137">Number of users in conflict</span></span>|
|<span data-ttu-id="8e3f5-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="8e3f5-138">errorCount</span></span>|<span data-ttu-id="8e3f5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3f5-139">Int32</span></span>|<span data-ttu-id="8e3f5-140">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="8e3f5-140">Number of error users</span></span>|
|<span data-ttu-id="8e3f5-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="8e3f5-141">failedCount</span></span>|<span data-ttu-id="8e3f5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3f5-142">Int32</span></span>|<span data-ttu-id="8e3f5-143">Número de usuários com falha</span><span class="sxs-lookup"><span data-stu-id="8e3f5-143">Number of failed users</span></span>|
|<span data-ttu-id="8e3f5-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8e3f5-144">notApplicableCount</span></span>|<span data-ttu-id="8e3f5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3f5-145">Int32</span></span>|<span data-ttu-id="8e3f5-146">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="8e3f5-146">Number of not applicable users</span></span>|
|<span data-ttu-id="8e3f5-147">successCount</span><span class="sxs-lookup"><span data-stu-id="8e3f5-147">successCount</span></span>|<span data-ttu-id="8e3f5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3f5-148">Int32</span></span>|<span data-ttu-id="8e3f5-149">Número de usuários com êxito</span><span class="sxs-lookup"><span data-stu-id="8e3f5-149">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="8e3f5-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3f5-150">Response</span></span>
<span data-ttu-id="8e3f5-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e3f5-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e3f5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e3f5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3f5-153">Request</span></span>
<span data-ttu-id="8e3f5-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e3f5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3f5-155">Response</span></span>
<span data-ttu-id="8e3f5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e3f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





