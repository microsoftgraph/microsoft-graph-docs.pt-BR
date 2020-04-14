---
title: Criar securityBaselineCategoryStateSummary
description: Criar um novo objeto securityBaselineCategoryStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99123c0dd864d4a876489b4da51ac3391a31af31
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381390"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="9a795-103">Criar securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="9a795-103">Create securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="9a795-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a795-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a795-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a795-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a795-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a795-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a795-107">Criar um novo objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9a795-107">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a795-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a795-108">Prerequisites</span></span>
<span data-ttu-id="9a795-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a795-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a795-111">Permission type</span></span>|<span data-ttu-id="9a795-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a795-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a795-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a795-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a795-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a795-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a795-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a795-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a795-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a795-116">Not supported.</span></span>|
|<span data-ttu-id="9a795-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a795-117">Application</span></span>|<span data-ttu-id="9a795-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a795-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a795-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a795-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9a795-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a795-120">Request headers</span></span>
|<span data-ttu-id="9a795-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a795-121">Header</span></span>|<span data-ttu-id="9a795-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a795-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a795-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a795-123">Authorization</span></span>|<span data-ttu-id="9a795-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a795-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a795-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a795-125">Accept</span></span>|<span data-ttu-id="9a795-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a795-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a795-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a795-127">Request body</span></span>
<span data-ttu-id="9a795-128">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineCategoryStateSummary.</span><span class="sxs-lookup"><span data-stu-id="9a795-128">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="9a795-129">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineCategoryStateSummary.</span><span class="sxs-lookup"><span data-stu-id="9a795-129">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="9a795-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a795-130">Property</span></span>|<span data-ttu-id="9a795-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a795-131">Type</span></span>|<span data-ttu-id="9a795-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a795-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a795-133">id</span><span class="sxs-lookup"><span data-stu-id="9a795-133">id</span></span>|<span data-ttu-id="9a795-134">String</span><span class="sxs-lookup"><span data-stu-id="9a795-134">String</span></span>|<span data-ttu-id="9a795-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="9a795-135">Unique identifier of the entity.</span></span> <span data-ttu-id="9a795-136">Herdado de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9a795-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9a795-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="9a795-137">secureCount</span></span>|<span data-ttu-id="9a795-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9a795-138">Int32</span></span>|<span data-ttu-id="9a795-139">Número de dispositivos seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9a795-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9a795-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="9a795-140">notSecureCount</span></span>|<span data-ttu-id="9a795-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9a795-141">Int32</span></span>|<span data-ttu-id="9a795-142">Número de dispositivos não seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9a795-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9a795-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="9a795-143">unknownCount</span></span>|<span data-ttu-id="9a795-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9a795-144">Int32</span></span>|<span data-ttu-id="9a795-145">Número de dispositivos desconhecidos herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9a795-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9a795-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="9a795-146">errorCount</span></span>|<span data-ttu-id="9a795-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9a795-147">Int32</span></span>|<span data-ttu-id="9a795-148">Número de dispositivos de erro herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9a795-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9a795-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9a795-149">conflictCount</span></span>|<span data-ttu-id="9a795-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9a795-150">Int32</span></span>|<span data-ttu-id="9a795-151">Número de dispositivos de conflito herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9a795-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9a795-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9a795-152">notApplicableCount</span></span>|<span data-ttu-id="9a795-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9a795-153">Int32</span></span>|<span data-ttu-id="9a795-154">Número de dispositivos não aplicáveis herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9a795-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9a795-155">displayName</span><span class="sxs-lookup"><span data-stu-id="9a795-155">displayName</span></span>|<span data-ttu-id="9a795-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a795-156">String</span></span>|<span data-ttu-id="9a795-157">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="9a795-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="9a795-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a795-158">Response</span></span>
<span data-ttu-id="9a795-159">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a795-159">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a795-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a795-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a795-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a795-161">Request</span></span>
<span data-ttu-id="9a795-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a795-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a795-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a795-163">Response</span></span>
<span data-ttu-id="9a795-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a795-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



