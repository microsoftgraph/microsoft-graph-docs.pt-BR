---
title: Criar securityBaselineCategoryStateSummary
description: Crie um novo objeto securityBaselineCategoryStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11fc148bcc4c25f36f315b7c15df2d0266b28845
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136570"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="35332-103">Criar securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="35332-103">Create securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="35332-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35332-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35332-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35332-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35332-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35332-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35332-107">Crie um novo [objeto securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="35332-107">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35332-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35332-108">Prerequisites</span></span>
<span data-ttu-id="35332-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35332-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35332-111">Permission type</span></span>|<span data-ttu-id="35332-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35332-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35332-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35332-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35332-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35332-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35332-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35332-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35332-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35332-116">Not supported.</span></span>|
|<span data-ttu-id="35332-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35332-117">Application</span></span>|<span data-ttu-id="35332-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35332-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35332-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35332-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="35332-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35332-120">Request headers</span></span>
|<span data-ttu-id="35332-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35332-121">Header</span></span>|<span data-ttu-id="35332-122">Valor</span><span class="sxs-lookup"><span data-stu-id="35332-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35332-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35332-123">Authorization</span></span>|<span data-ttu-id="35332-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35332-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35332-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35332-125">Accept</span></span>|<span data-ttu-id="35332-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35332-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35332-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35332-127">Request body</span></span>
<span data-ttu-id="35332-128">No corpo da solicitação, fornece uma representação JSON para o objeto securityBaselineCategoryStateSummary.</span><span class="sxs-lookup"><span data-stu-id="35332-128">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="35332-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o securityBaselineCategoryStateSummary.</span><span class="sxs-lookup"><span data-stu-id="35332-129">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="35332-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35332-130">Property</span></span>|<span data-ttu-id="35332-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="35332-131">Type</span></span>|<span data-ttu-id="35332-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="35332-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35332-133">id</span><span class="sxs-lookup"><span data-stu-id="35332-133">id</span></span>|<span data-ttu-id="35332-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35332-134">String</span></span>|<span data-ttu-id="35332-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="35332-135">Unique identifier of the entity.</span></span> <span data-ttu-id="35332-136">Herdado [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="35332-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="35332-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="35332-137">secureCount</span></span>|<span data-ttu-id="35332-138">Int32</span><span class="sxs-lookup"><span data-stu-id="35332-138">Int32</span></span>|<span data-ttu-id="35332-139">Número de dispositivos seguros Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="35332-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="35332-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="35332-140">notSecureCount</span></span>|<span data-ttu-id="35332-141">Int32</span><span class="sxs-lookup"><span data-stu-id="35332-141">Int32</span></span>|<span data-ttu-id="35332-142">Número de dispositivos não seguros Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="35332-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="35332-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="35332-143">unknownCount</span></span>|<span data-ttu-id="35332-144">Int32</span><span class="sxs-lookup"><span data-stu-id="35332-144">Int32</span></span>|<span data-ttu-id="35332-145">Número de dispositivos desconhecidos Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="35332-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="35332-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="35332-146">errorCount</span></span>|<span data-ttu-id="35332-147">Int32</span><span class="sxs-lookup"><span data-stu-id="35332-147">Int32</span></span>|<span data-ttu-id="35332-148">Número de dispositivos de erro Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="35332-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="35332-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="35332-149">conflictCount</span></span>|<span data-ttu-id="35332-150">Int32</span><span class="sxs-lookup"><span data-stu-id="35332-150">Int32</span></span>|<span data-ttu-id="35332-151">Número de dispositivos de conflito Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="35332-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="35332-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="35332-152">notApplicableCount</span></span>|<span data-ttu-id="35332-153">Int32</span><span class="sxs-lookup"><span data-stu-id="35332-153">Int32</span></span>|<span data-ttu-id="35332-154">Número de dispositivos não aplicáveis Herdados [de securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="35332-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="35332-155">displayName</span><span class="sxs-lookup"><span data-stu-id="35332-155">displayName</span></span>|<span data-ttu-id="35332-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35332-156">String</span></span>|<span data-ttu-id="35332-157">O nome da categoria</span><span class="sxs-lookup"><span data-stu-id="35332-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="35332-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="35332-158">Response</span></span>
<span data-ttu-id="35332-159">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35332-159">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35332-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35332-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="35332-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35332-161">Request</span></span>
<span data-ttu-id="35332-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35332-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="35332-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="35332-163">Response</span></span>
<span data-ttu-id="35332-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35332-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




