---
title: Atualizar securityBaselineCategoryStateSummary
description: Atualiza as propriedades de um objeto securityBaselineCategoryStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04f014cc683bdc098a54e1571f4cb2a8b8a1ee2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022530"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="74441-103">Atualizar securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="74441-103">Update securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="74441-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74441-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74441-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74441-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74441-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74441-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74441-107">Atualiza as propriedades de um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="74441-107">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74441-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74441-108">Prerequisites</span></span>
<span data-ttu-id="74441-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74441-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74441-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74441-111">Permission type</span></span>|<span data-ttu-id="74441-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74441-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74441-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74441-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74441-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74441-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74441-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74441-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74441-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74441-116">Not supported.</span></span>|
|<span data-ttu-id="74441-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74441-117">Application</span></span>|<span data-ttu-id="74441-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74441-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74441-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74441-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="74441-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74441-120">Request headers</span></span>
|<span data-ttu-id="74441-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74441-121">Header</span></span>|<span data-ttu-id="74441-122">Valor</span><span class="sxs-lookup"><span data-stu-id="74441-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74441-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="74441-123">Authorization</span></span>|<span data-ttu-id="74441-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74441-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74441-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74441-125">Accept</span></span>|<span data-ttu-id="74441-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74441-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74441-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74441-127">Request body</span></span>
<span data-ttu-id="74441-128">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="74441-128">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="74441-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="74441-129">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="74441-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74441-130">Property</span></span>|<span data-ttu-id="74441-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="74441-131">Type</span></span>|<span data-ttu-id="74441-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="74441-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74441-133">id</span><span class="sxs-lookup"><span data-stu-id="74441-133">id</span></span>|<span data-ttu-id="74441-134">String</span><span class="sxs-lookup"><span data-stu-id="74441-134">String</span></span>|<span data-ttu-id="74441-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="74441-135">Unique identifier of the entity.</span></span> <span data-ttu-id="74441-136">Herdado de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="74441-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="74441-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="74441-137">secureCount</span></span>|<span data-ttu-id="74441-138">Int32</span><span class="sxs-lookup"><span data-stu-id="74441-138">Int32</span></span>|<span data-ttu-id="74441-139">Número de dispositivos seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="74441-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="74441-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="74441-140">notSecureCount</span></span>|<span data-ttu-id="74441-141">Int32</span><span class="sxs-lookup"><span data-stu-id="74441-141">Int32</span></span>|<span data-ttu-id="74441-142">Número de dispositivos não seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="74441-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="74441-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="74441-143">unknownCount</span></span>|<span data-ttu-id="74441-144">Int32</span><span class="sxs-lookup"><span data-stu-id="74441-144">Int32</span></span>|<span data-ttu-id="74441-145">Número de dispositivos desconhecidos herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="74441-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="74441-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="74441-146">errorCount</span></span>|<span data-ttu-id="74441-147">Int32</span><span class="sxs-lookup"><span data-stu-id="74441-147">Int32</span></span>|<span data-ttu-id="74441-148">Número de dispositivos de erro herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="74441-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="74441-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="74441-149">conflictCount</span></span>|<span data-ttu-id="74441-150">Int32</span><span class="sxs-lookup"><span data-stu-id="74441-150">Int32</span></span>|<span data-ttu-id="74441-151">Número de dispositivos de conflito herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="74441-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="74441-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="74441-152">notApplicableCount</span></span>|<span data-ttu-id="74441-153">Int32</span><span class="sxs-lookup"><span data-stu-id="74441-153">Int32</span></span>|<span data-ttu-id="74441-154">Número de dispositivos não aplicáveis herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="74441-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="74441-155">displayName</span><span class="sxs-lookup"><span data-stu-id="74441-155">displayName</span></span>|<span data-ttu-id="74441-156">String</span><span class="sxs-lookup"><span data-stu-id="74441-156">String</span></span>|<span data-ttu-id="74441-157">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="74441-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="74441-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="74441-158">Response</span></span>
<span data-ttu-id="74441-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74441-159">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74441-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74441-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="74441-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74441-161">Request</span></span>
<span data-ttu-id="74441-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74441-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74441-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="74441-163">Response</span></span>
<span data-ttu-id="74441-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74441-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






