---
title: Criar securityBaselineCategoryStateSummary
description: Criar um novo objeto securityBaselineCategoryStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b52b8f3c84f80831710667c6f58e0df50f5804cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470263"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="a0435-103">Criar securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="a0435-103">Create securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="a0435-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a0435-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0435-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0435-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0435-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0435-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0435-107">Criar um novo objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a0435-107">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0435-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0435-108">Prerequisites</span></span>
<span data-ttu-id="a0435-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0435-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0435-111">Permission type</span></span>|<span data-ttu-id="a0435-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0435-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0435-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0435-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0435-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0435-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0435-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0435-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0435-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0435-116">Not supported.</span></span>|
|<span data-ttu-id="a0435-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0435-117">Application</span></span>|<span data-ttu-id="a0435-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0435-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0435-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0435-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a0435-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0435-120">Request headers</span></span>
|<span data-ttu-id="a0435-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0435-121">Header</span></span>|<span data-ttu-id="a0435-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0435-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0435-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0435-123">Authorization</span></span>|<span data-ttu-id="a0435-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0435-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0435-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0435-125">Accept</span></span>|<span data-ttu-id="a0435-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0435-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0435-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0435-127">Request body</span></span>
<span data-ttu-id="a0435-128">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineCategoryStateSummary.</span><span class="sxs-lookup"><span data-stu-id="a0435-128">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="a0435-129">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineCategoryStateSummary.</span><span class="sxs-lookup"><span data-stu-id="a0435-129">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="a0435-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0435-130">Property</span></span>|<span data-ttu-id="a0435-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0435-131">Type</span></span>|<span data-ttu-id="a0435-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0435-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0435-133">id</span><span class="sxs-lookup"><span data-stu-id="a0435-133">id</span></span>|<span data-ttu-id="a0435-134">String</span><span class="sxs-lookup"><span data-stu-id="a0435-134">String</span></span>|<span data-ttu-id="a0435-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0435-135">Unique identifier of the entity.</span></span> <span data-ttu-id="a0435-136">Herdado de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a0435-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a0435-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="a0435-137">secureCount</span></span>|<span data-ttu-id="a0435-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a0435-138">Int32</span></span>|<span data-ttu-id="a0435-139">Número de dispositivos seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a0435-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a0435-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="a0435-140">notSecureCount</span></span>|<span data-ttu-id="a0435-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a0435-141">Int32</span></span>|<span data-ttu-id="a0435-142">Número de dispositivos não seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a0435-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a0435-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="a0435-143">unknownCount</span></span>|<span data-ttu-id="a0435-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a0435-144">Int32</span></span>|<span data-ttu-id="a0435-145">Número de dispositivos desconhecidos herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a0435-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a0435-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="a0435-146">errorCount</span></span>|<span data-ttu-id="a0435-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a0435-147">Int32</span></span>|<span data-ttu-id="a0435-148">Número de dispositivos de erro herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a0435-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a0435-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="a0435-149">conflictCount</span></span>|<span data-ttu-id="a0435-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a0435-150">Int32</span></span>|<span data-ttu-id="a0435-151">Número de dispositivos de conflito herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a0435-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a0435-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a0435-152">notApplicableCount</span></span>|<span data-ttu-id="a0435-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a0435-153">Int32</span></span>|<span data-ttu-id="a0435-154">Número de dispositivos não aplicáveis herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="a0435-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="a0435-155">displayName</span><span class="sxs-lookup"><span data-stu-id="a0435-155">displayName</span></span>|<span data-ttu-id="a0435-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0435-156">String</span></span>|<span data-ttu-id="a0435-157">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="a0435-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="a0435-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0435-158">Response</span></span>
<span data-ttu-id="a0435-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0435-159">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0435-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0435-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0435-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0435-161">Request</span></span>
<span data-ttu-id="a0435-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0435-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
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

### <a name="response"></a><span data-ttu-id="a0435-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0435-163">Response</span></span>
<span data-ttu-id="a0435-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0435-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





