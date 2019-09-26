---
title: Atualizar securityBaselineStateSummary
description: Atualiza as propriedades de um objeto securityBaselineStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5141ce21ce2d0cee08e23a8f12e50c98551bc841
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179450"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="f274c-103">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="f274c-103">Update securityBaselineStateSummary</span></span>

> <span data-ttu-id="f274c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f274c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f274c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f274c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f274c-106">Atualiza as propriedades de um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f274c-106">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f274c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f274c-107">Prerequisites</span></span>
<span data-ttu-id="f274c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f274c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f274c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f274c-110">Permission type</span></span>|<span data-ttu-id="f274c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f274c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f274c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f274c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f274c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f274c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f274c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f274c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f274c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f274c-115">Not supported.</span></span>|
|<span data-ttu-id="f274c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f274c-116">Application</span></span>|<span data-ttu-id="f274c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f274c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f274c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f274c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="f274c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f274c-119">Request headers</span></span>
|<span data-ttu-id="f274c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f274c-120">Header</span></span>|<span data-ttu-id="f274c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f274c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f274c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f274c-122">Authorization</span></span>|<span data-ttu-id="f274c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f274c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f274c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f274c-124">Accept</span></span>|<span data-ttu-id="f274c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f274c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f274c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f274c-126">Request body</span></span>
<span data-ttu-id="f274c-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f274c-127">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="f274c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f274c-128">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="f274c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f274c-129">Property</span></span>|<span data-ttu-id="f274c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f274c-130">Type</span></span>|<span data-ttu-id="f274c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f274c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f274c-132">id</span><span class="sxs-lookup"><span data-stu-id="f274c-132">id</span></span>|<span data-ttu-id="f274c-133">String</span><span class="sxs-lookup"><span data-stu-id="f274c-133">String</span></span>|<span data-ttu-id="f274c-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="f274c-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f274c-135">secureCount</span><span class="sxs-lookup"><span data-stu-id="f274c-135">secureCount</span></span>|<span data-ttu-id="f274c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f274c-136">Int32</span></span>|<span data-ttu-id="f274c-137">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="f274c-137">Number of secure devices</span></span>|
|<span data-ttu-id="f274c-138">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="f274c-138">notSecureCount</span></span>|<span data-ttu-id="f274c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f274c-139">Int32</span></span>|<span data-ttu-id="f274c-140">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="f274c-140">Number of not secure devices</span></span>|
|<span data-ttu-id="f274c-141">unknownCount</span><span class="sxs-lookup"><span data-stu-id="f274c-141">unknownCount</span></span>|<span data-ttu-id="f274c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f274c-142">Int32</span></span>|<span data-ttu-id="f274c-143">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="f274c-143">Number of unknown devices</span></span>|
|<span data-ttu-id="f274c-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="f274c-144">errorCount</span></span>|<span data-ttu-id="f274c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f274c-145">Int32</span></span>|<span data-ttu-id="f274c-146">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="f274c-146">Number of error devices</span></span>|
|<span data-ttu-id="f274c-147">conflictCount</span><span class="sxs-lookup"><span data-stu-id="f274c-147">conflictCount</span></span>|<span data-ttu-id="f274c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f274c-148">Int32</span></span>|<span data-ttu-id="f274c-149">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="f274c-149">Number of conflict devices</span></span>|
|<span data-ttu-id="f274c-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f274c-150">notApplicableCount</span></span>|<span data-ttu-id="f274c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f274c-151">Int32</span></span>|<span data-ttu-id="f274c-152">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f274c-152">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="f274c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f274c-153">Response</span></span>
<span data-ttu-id="f274c-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f274c-154">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f274c-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f274c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="f274c-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f274c-156">Request</span></span>
<span data-ttu-id="f274c-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f274c-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f274c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f274c-158">Response</span></span>
<span data-ttu-id="f274c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f274c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




