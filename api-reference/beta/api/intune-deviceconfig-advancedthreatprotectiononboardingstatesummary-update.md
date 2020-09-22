---
title: Atualizar Navegaçãoadvancedthreatprotectiononboardingstatesummary
description: Atualiza as propriedades de um objeto Navegaçãoadvancedthreatprotectiononboardingstatesummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 544c7f27b0f498e86b66ef4d72112f75321c90b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990330"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="c900c-103">Atualizar Navegaçãoadvancedthreatprotectiononboardingstatesummary</span><span class="sxs-lookup"><span data-stu-id="c900c-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

<span data-ttu-id="c900c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c900c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c900c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c900c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c900c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c900c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c900c-107">Atualiza as propriedades de um objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c900c-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c900c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c900c-108">Prerequisites</span></span>
<span data-ttu-id="c900c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c900c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c900c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c900c-111">Permission type</span></span>|<span data-ttu-id="c900c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c900c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c900c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c900c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c900c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c900c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c900c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c900c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c900c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c900c-116">Not supported.</span></span>|
|<span data-ttu-id="c900c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c900c-117">Application</span></span>|<span data-ttu-id="c900c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c900c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c900c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c900c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c900c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c900c-120">Request headers</span></span>
|<span data-ttu-id="c900c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c900c-121">Header</span></span>|<span data-ttu-id="c900c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c900c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c900c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c900c-123">Authorization</span></span>|<span data-ttu-id="c900c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c900c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c900c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c900c-125">Accept</span></span>|<span data-ttu-id="c900c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c900c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c900c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c900c-127">Request body</span></span>
<span data-ttu-id="c900c-128">No corpo da solicitação, forneça uma representação JSON do objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c900c-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="c900c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c900c-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="c900c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c900c-130">Property</span></span>|<span data-ttu-id="c900c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c900c-131">Type</span></span>|<span data-ttu-id="c900c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c900c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c900c-133">id</span><span class="sxs-lookup"><span data-stu-id="c900c-133">id</span></span>|<span data-ttu-id="c900c-134">String</span><span class="sxs-lookup"><span data-stu-id="c900c-134">String</span></span>|<span data-ttu-id="c900c-135">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="c900c-135">Unique Identifier</span></span>|
|<span data-ttu-id="c900c-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c900c-136">unknownDeviceCount</span></span>|<span data-ttu-id="c900c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c900c-137">Int32</span></span>|<span data-ttu-id="c900c-138">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="c900c-138">Number of unknown devices</span></span>|
|<span data-ttu-id="c900c-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c900c-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="c900c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c900c-140">Int32</span></span>|<span data-ttu-id="c900c-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="c900c-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="c900c-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c900c-142">compliantDeviceCount</span></span>|<span data-ttu-id="c900c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c900c-143">Int32</span></span>|<span data-ttu-id="c900c-144">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="c900c-144">Number of compliant devices</span></span>|
|<span data-ttu-id="c900c-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c900c-145">remediatedDeviceCount</span></span>|<span data-ttu-id="c900c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c900c-146">Int32</span></span>|<span data-ttu-id="c900c-147">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="c900c-147">Number of remediated devices</span></span>|
|<span data-ttu-id="c900c-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c900c-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c900c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c900c-149">Int32</span></span>|<span data-ttu-id="c900c-150">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="c900c-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c900c-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c900c-151">errorDeviceCount</span></span>|<span data-ttu-id="c900c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c900c-152">Int32</span></span>|<span data-ttu-id="c900c-153">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="c900c-153">Number of error devices</span></span>|
|<span data-ttu-id="c900c-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c900c-154">conflictDeviceCount</span></span>|<span data-ttu-id="c900c-155">Int32</span><span class="sxs-lookup"><span data-stu-id="c900c-155">Int32</span></span>|<span data-ttu-id="c900c-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="c900c-156">Number of conflict devices</span></span>|
|<span data-ttu-id="c900c-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c900c-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="c900c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c900c-158">Int32</span></span>|<span data-ttu-id="c900c-159">Número de dispositivos não atribuídos</span><span class="sxs-lookup"><span data-stu-id="c900c-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="c900c-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="c900c-160">Response</span></span>
<span data-ttu-id="c900c-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c900c-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c900c-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c900c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c900c-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c900c-163">Request</span></span>
<span data-ttu-id="c900c-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c900c-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```

### <a name="response"></a><span data-ttu-id="c900c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="c900c-165">Response</span></span>
<span data-ttu-id="c900c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c900c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "74089602-9602-7408-0296-087402960874",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```






