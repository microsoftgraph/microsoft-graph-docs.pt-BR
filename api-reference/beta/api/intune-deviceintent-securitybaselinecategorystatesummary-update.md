---
title: Atualizar securityBaselineCategoryStateSummary
description: Atualiza as propriedades de um objeto securityBaselineCategoryStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93168dc57fc9f70f2ba15017d6c6a8cf3d2b34e7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179485"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="38ba2-103">Atualizar securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="38ba2-103">Update securityBaselineCategoryStateSummary</span></span>

> <span data-ttu-id="38ba2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38ba2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38ba2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38ba2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38ba2-106">Atualiza as propriedades de um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="38ba2-106">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38ba2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38ba2-107">Prerequisites</span></span>
<span data-ttu-id="38ba2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38ba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38ba2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38ba2-110">Permission type</span></span>|<span data-ttu-id="38ba2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38ba2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38ba2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38ba2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38ba2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ba2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38ba2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38ba2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38ba2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38ba2-115">Not supported.</span></span>|
|<span data-ttu-id="38ba2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38ba2-116">Application</span></span>|<span data-ttu-id="38ba2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ba2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38ba2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38ba2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="38ba2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38ba2-119">Request headers</span></span>
|<span data-ttu-id="38ba2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38ba2-120">Header</span></span>|<span data-ttu-id="38ba2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="38ba2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38ba2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38ba2-122">Authorization</span></span>|<span data-ttu-id="38ba2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38ba2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38ba2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38ba2-124">Accept</span></span>|<span data-ttu-id="38ba2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38ba2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38ba2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38ba2-126">Request body</span></span>
<span data-ttu-id="38ba2-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="38ba2-127">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="38ba2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="38ba2-128">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="38ba2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38ba2-129">Property</span></span>|<span data-ttu-id="38ba2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="38ba2-130">Type</span></span>|<span data-ttu-id="38ba2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="38ba2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38ba2-132">id</span><span class="sxs-lookup"><span data-stu-id="38ba2-132">id</span></span>|<span data-ttu-id="38ba2-133">String</span><span class="sxs-lookup"><span data-stu-id="38ba2-133">String</span></span>|<span data-ttu-id="38ba2-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="38ba2-134">Unique identifier of the entity.</span></span> <span data-ttu-id="38ba2-135">Herdado de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="38ba2-135">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="38ba2-136">secureCount</span><span class="sxs-lookup"><span data-stu-id="38ba2-136">secureCount</span></span>|<span data-ttu-id="38ba2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="38ba2-137">Int32</span></span>|<span data-ttu-id="38ba2-138">Número de dispositivos seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="38ba2-138">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="38ba2-139">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="38ba2-139">notSecureCount</span></span>|<span data-ttu-id="38ba2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="38ba2-140">Int32</span></span>|<span data-ttu-id="38ba2-141">Número de dispositivos não seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="38ba2-141">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="38ba2-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="38ba2-142">unknownCount</span></span>|<span data-ttu-id="38ba2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="38ba2-143">Int32</span></span>|<span data-ttu-id="38ba2-144">Número de dispositivos desconhecidos herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="38ba2-144">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="38ba2-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="38ba2-145">errorCount</span></span>|<span data-ttu-id="38ba2-146">Int32</span><span class="sxs-lookup"><span data-stu-id="38ba2-146">Int32</span></span>|<span data-ttu-id="38ba2-147">Número de dispositivos de erro herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="38ba2-147">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="38ba2-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="38ba2-148">conflictCount</span></span>|<span data-ttu-id="38ba2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="38ba2-149">Int32</span></span>|<span data-ttu-id="38ba2-150">Número de dispositivos de conflito herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="38ba2-150">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="38ba2-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="38ba2-151">notApplicableCount</span></span>|<span data-ttu-id="38ba2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="38ba2-152">Int32</span></span>|<span data-ttu-id="38ba2-153">Número de dispositivos não aplicáveis herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="38ba2-153">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="38ba2-154">displayName</span><span class="sxs-lookup"><span data-stu-id="38ba2-154">displayName</span></span>|<span data-ttu-id="38ba2-155">String</span><span class="sxs-lookup"><span data-stu-id="38ba2-155">String</span></span>|<span data-ttu-id="38ba2-156">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="38ba2-156">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="38ba2-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ba2-157">Response</span></span>
<span data-ttu-id="38ba2-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38ba2-158">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ba2-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38ba2-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="38ba2-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38ba2-160">Request</span></span>
<span data-ttu-id="38ba2-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38ba2-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="38ba2-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="38ba2-162">Response</span></span>
<span data-ttu-id="38ba2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38ba2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```




