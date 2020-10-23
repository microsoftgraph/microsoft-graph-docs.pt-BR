---
title: Atualizar securityBaselineStateSummary
description: Atualiza as propriedades de um objeto securityBaselineStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cbad348157ddeac184ec6663d3558535418d2a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729984"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="97d47-103">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="97d47-103">Update securityBaselineStateSummary</span></span>

<span data-ttu-id="97d47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97d47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97d47-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97d47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97d47-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97d47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d47-107">Atualiza as propriedades de um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="97d47-107">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97d47-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97d47-108">Prerequisites</span></span>
<span data-ttu-id="97d47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97d47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97d47-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97d47-111">Permission type</span></span>|<span data-ttu-id="97d47-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97d47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97d47-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97d47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97d47-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d47-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97d47-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97d47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97d47-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97d47-116">Not supported.</span></span>|
|<span data-ttu-id="97d47-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97d47-117">Application</span></span>|<span data-ttu-id="97d47-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d47-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97d47-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97d47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="97d47-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97d47-120">Request headers</span></span>
|<span data-ttu-id="97d47-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97d47-121">Header</span></span>|<span data-ttu-id="97d47-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97d47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97d47-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97d47-123">Authorization</span></span>|<span data-ttu-id="97d47-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97d47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97d47-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97d47-125">Accept</span></span>|<span data-ttu-id="97d47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97d47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97d47-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97d47-127">Request body</span></span>
<span data-ttu-id="97d47-128">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="97d47-128">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="97d47-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="97d47-129">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="97d47-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97d47-130">Property</span></span>|<span data-ttu-id="97d47-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97d47-131">Type</span></span>|<span data-ttu-id="97d47-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97d47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d47-133">id</span><span class="sxs-lookup"><span data-stu-id="97d47-133">id</span></span>|<span data-ttu-id="97d47-134">String</span><span class="sxs-lookup"><span data-stu-id="97d47-134">String</span></span>|<span data-ttu-id="97d47-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="97d47-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="97d47-136">secureCount</span><span class="sxs-lookup"><span data-stu-id="97d47-136">secureCount</span></span>|<span data-ttu-id="97d47-137">Int32</span><span class="sxs-lookup"><span data-stu-id="97d47-137">Int32</span></span>|<span data-ttu-id="97d47-138">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="97d47-138">Number of secure devices</span></span>|
|<span data-ttu-id="97d47-139">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="97d47-139">notSecureCount</span></span>|<span data-ttu-id="97d47-140">Int32</span><span class="sxs-lookup"><span data-stu-id="97d47-140">Int32</span></span>|<span data-ttu-id="97d47-141">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="97d47-141">Number of not secure devices</span></span>|
|<span data-ttu-id="97d47-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="97d47-142">unknownCount</span></span>|<span data-ttu-id="97d47-143">Int32</span><span class="sxs-lookup"><span data-stu-id="97d47-143">Int32</span></span>|<span data-ttu-id="97d47-144">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="97d47-144">Number of unknown devices</span></span>|
|<span data-ttu-id="97d47-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="97d47-145">errorCount</span></span>|<span data-ttu-id="97d47-146">Int32</span><span class="sxs-lookup"><span data-stu-id="97d47-146">Int32</span></span>|<span data-ttu-id="97d47-147">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="97d47-147">Number of error devices</span></span>|
|<span data-ttu-id="97d47-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="97d47-148">conflictCount</span></span>|<span data-ttu-id="97d47-149">Int32</span><span class="sxs-lookup"><span data-stu-id="97d47-149">Int32</span></span>|<span data-ttu-id="97d47-150">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="97d47-150">Number of conflict devices</span></span>|
|<span data-ttu-id="97d47-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="97d47-151">notApplicableCount</span></span>|<span data-ttu-id="97d47-152">Int32</span><span class="sxs-lookup"><span data-stu-id="97d47-152">Int32</span></span>|<span data-ttu-id="97d47-153">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="97d47-153">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="97d47-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d47-154">Response</span></span>
<span data-ttu-id="97d47-155">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97d47-155">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97d47-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97d47-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="97d47-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97d47-157">Request</span></span>
<span data-ttu-id="97d47-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97d47-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```

### <a name="response"></a><span data-ttu-id="97d47-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d47-159">Response</span></span>
<span data-ttu-id="97d47-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97d47-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```





