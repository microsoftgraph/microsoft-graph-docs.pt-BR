---
title: Atualizar securityBaselineCategoryStateSummary
description: Atualiza as propriedades de um objeto securityBaselineCategoryStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07b87a57cc9b54f72c306289d82ceac5cf8ced72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470249"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="9c62f-103">Atualizar securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="9c62f-103">Update securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="9c62f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9c62f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c62f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c62f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c62f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c62f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c62f-107">Atualiza as propriedades de um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9c62f-107">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c62f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c62f-108">Prerequisites</span></span>
<span data-ttu-id="9c62f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c62f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c62f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c62f-111">Permission type</span></span>|<span data-ttu-id="9c62f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c62f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c62f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c62f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c62f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c62f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c62f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c62f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c62f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c62f-116">Not supported.</span></span>|
|<span data-ttu-id="9c62f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c62f-117">Application</span></span>|<span data-ttu-id="9c62f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c62f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c62f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c62f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="9c62f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c62f-120">Request headers</span></span>
|<span data-ttu-id="9c62f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c62f-121">Header</span></span>|<span data-ttu-id="9c62f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9c62f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c62f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c62f-123">Authorization</span></span>|<span data-ttu-id="9c62f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c62f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c62f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c62f-125">Accept</span></span>|<span data-ttu-id="9c62f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c62f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c62f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c62f-127">Request body</span></span>
<span data-ttu-id="9c62f-128">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9c62f-128">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="9c62f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9c62f-129">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="9c62f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c62f-130">Property</span></span>|<span data-ttu-id="9c62f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c62f-131">Type</span></span>|<span data-ttu-id="9c62f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c62f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c62f-133">id</span><span class="sxs-lookup"><span data-stu-id="9c62f-133">id</span></span>|<span data-ttu-id="9c62f-134">String</span><span class="sxs-lookup"><span data-stu-id="9c62f-134">String</span></span>|<span data-ttu-id="9c62f-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="9c62f-135">Unique identifier of the entity.</span></span> <span data-ttu-id="9c62f-136">Herdado de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c62f-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9c62f-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="9c62f-137">secureCount</span></span>|<span data-ttu-id="9c62f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9c62f-138">Int32</span></span>|<span data-ttu-id="9c62f-139">Número de dispositivos seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c62f-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9c62f-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="9c62f-140">notSecureCount</span></span>|<span data-ttu-id="9c62f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9c62f-141">Int32</span></span>|<span data-ttu-id="9c62f-142">Número de dispositivos não seguros herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c62f-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9c62f-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="9c62f-143">unknownCount</span></span>|<span data-ttu-id="9c62f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9c62f-144">Int32</span></span>|<span data-ttu-id="9c62f-145">Número de dispositivos desconhecidos herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c62f-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9c62f-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="9c62f-146">errorCount</span></span>|<span data-ttu-id="9c62f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9c62f-147">Int32</span></span>|<span data-ttu-id="9c62f-148">Número de dispositivos de erro herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c62f-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9c62f-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9c62f-149">conflictCount</span></span>|<span data-ttu-id="9c62f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9c62f-150">Int32</span></span>|<span data-ttu-id="9c62f-151">Número de dispositivos de conflito herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c62f-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9c62f-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9c62f-152">notApplicableCount</span></span>|<span data-ttu-id="9c62f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9c62f-153">Int32</span></span>|<span data-ttu-id="9c62f-154">Número de dispositivos não aplicáveis herdados de [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c62f-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="9c62f-155">displayName</span><span class="sxs-lookup"><span data-stu-id="9c62f-155">displayName</span></span>|<span data-ttu-id="9c62f-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c62f-156">String</span></span>|<span data-ttu-id="9c62f-157">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="9c62f-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="9c62f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c62f-158">Response</span></span>
<span data-ttu-id="9c62f-159">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c62f-159">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c62f-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c62f-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c62f-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c62f-161">Request</span></span>
<span data-ttu-id="9c62f-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c62f-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c62f-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c62f-163">Response</span></span>
<span data-ttu-id="9c62f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c62f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





