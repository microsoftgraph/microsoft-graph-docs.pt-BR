---
title: Atualizar deviceManagementIntentUserStateSummary
description: Atualiza as propriedades de um objeto deviceManagementIntentUserStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f43e8499b341b30b475ed3ccc9a1954056c6bb21
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43325607"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="552c1-103">Atualizar deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="552c1-103">Update deviceManagementIntentUserStateSummary</span></span>

<span data-ttu-id="552c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="552c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="552c1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="552c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="552c1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="552c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="552c1-107">Atualiza as propriedades de um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="552c1-107">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="552c1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="552c1-108">Prerequisites</span></span>
<span data-ttu-id="552c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="552c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="552c1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="552c1-111">Permission type</span></span>|<span data-ttu-id="552c1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="552c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="552c1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="552c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="552c1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552c1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="552c1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="552c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="552c1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="552c1-116">Not supported.</span></span>|
|<span data-ttu-id="552c1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="552c1-117">Application</span></span>|<span data-ttu-id="552c1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552c1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="552c1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="552c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="552c1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="552c1-120">Request headers</span></span>
|<span data-ttu-id="552c1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="552c1-121">Header</span></span>|<span data-ttu-id="552c1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="552c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="552c1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="552c1-123">Authorization</span></span>|<span data-ttu-id="552c1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="552c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="552c1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="552c1-125">Accept</span></span>|<span data-ttu-id="552c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="552c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="552c1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="552c1-127">Request body</span></span>
<span data-ttu-id="552c1-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="552c1-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="552c1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="552c1-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="552c1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="552c1-130">Property</span></span>|<span data-ttu-id="552c1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="552c1-131">Type</span></span>|<span data-ttu-id="552c1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="552c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="552c1-133">id</span><span class="sxs-lookup"><span data-stu-id="552c1-133">id</span></span>|<span data-ttu-id="552c1-134">String</span><span class="sxs-lookup"><span data-stu-id="552c1-134">String</span></span>|<span data-ttu-id="552c1-135">A ID</span><span class="sxs-lookup"><span data-stu-id="552c1-135">The ID</span></span>|
|<span data-ttu-id="552c1-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="552c1-136">conflictCount</span></span>|<span data-ttu-id="552c1-137">Int32</span><span class="sxs-lookup"><span data-stu-id="552c1-137">Int32</span></span>|<span data-ttu-id="552c1-138">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="552c1-138">Number of users in conflict</span></span>|
|<span data-ttu-id="552c1-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="552c1-139">errorCount</span></span>|<span data-ttu-id="552c1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="552c1-140">Int32</span></span>|<span data-ttu-id="552c1-141">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="552c1-141">Number of error users</span></span>|
|<span data-ttu-id="552c1-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="552c1-142">failedCount</span></span>|<span data-ttu-id="552c1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="552c1-143">Int32</span></span>|<span data-ttu-id="552c1-144">Número de usuários com falha</span><span class="sxs-lookup"><span data-stu-id="552c1-144">Number of failed users</span></span>|
|<span data-ttu-id="552c1-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="552c1-145">notApplicableCount</span></span>|<span data-ttu-id="552c1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="552c1-146">Int32</span></span>|<span data-ttu-id="552c1-147">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="552c1-147">Number of not applicable users</span></span>|
|<span data-ttu-id="552c1-148">successCount</span><span class="sxs-lookup"><span data-stu-id="552c1-148">successCount</span></span>|<span data-ttu-id="552c1-149">Int32</span><span class="sxs-lookup"><span data-stu-id="552c1-149">Int32</span></span>|<span data-ttu-id="552c1-150">Número de usuários com êxito</span><span class="sxs-lookup"><span data-stu-id="552c1-150">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="552c1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="552c1-151">Response</span></span>
<span data-ttu-id="552c1-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="552c1-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="552c1-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="552c1-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="552c1-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="552c1-154">Request</span></span>
<span data-ttu-id="552c1-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="552c1-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="552c1-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="552c1-156">Response</span></span>
<span data-ttu-id="552c1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="552c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



